How to add Extra classes is in the Vafpress Docs

The Folders provided go in a folder called `vp_custom_fields` - can be called anything so long as it's changed in the snippet. Folder can go anywhere, just point to it in the snippet where I have a constant of THEME_FRAMEWORK_DIR.

here is how I added:


	// Directories for Custom Fields Register
	$vpfs = VP_FileSystem::instance();
	$vpfs->add_directories( 'views', THEME_FRAMEWORK_DIR . '/vp_custom_fields/views');
	VP_AutoLoader::add_directories(THEME_FRAMEWORK_DIR . '/vp_custom_fields/classes', 'VP_');

## Adding a taxonomy

Gives checkboxes of taxonomy categories associated with the custom post types

     array(
        'type' => 'taxonomy',
        'heading' => 'Categories',
        'taxonomy' => 'category',
        'param_name' => 'terms',
        ),
        
        
## Media field

Returns the id rather then the url

    array(
				'type' => 'media',
				'name' => 'upload',
				'label' => __('Image', 'ZX_TEXTDOMAIN'),
				'description' => __('mp4 recommended', 'ZX_TEXTDOMAIN'),
				'default' => 'http://placehold.it/70x70',
				);
				
More to come
