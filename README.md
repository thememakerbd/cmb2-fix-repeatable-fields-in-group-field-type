#cmb2-fix-repeatable-fields-in-group-field-type
Fix Wordpress cmb2 plugin repeatable fields issue in group field


In CMB2 i was found a issue with multi repeatable fields in Group field type. Then i research on it. but i didn't found any solution for that. Finaly I fix this issue my self. 

Step:

1) You need to replace cmb2.js in cmb2/js folder with my cmb2.js
2) In cmb2/includes/CMB2_JS.php at line 79 you need replace wp_enqueue_script( self::$handle, CMB2_Utils::url( "js/cmb2{min}.js" ), $dependencies, CMB2_VERSION, true ); to wp_enqueue_script( self::$handle, CMB2_Utils::url( "js/cmb2.js" ), $dependencies, CMB2_VERSION, true );

And Done.
