How to add Extra classes is in the Vafpress Docs

here is how I added

# Directories for Custom Fields Register
$vpfs = VP_FileSystem::instance();
$vpfs->add_directories( 'views', THEME_FRAMEWORK_DIR . '/vp_custom_fields/views');
VP_AutoLoader::add_directories(THEME_FRAMEWORK_DIR . '/vp_custom_fields/classes', 'VP_');

# Adding a taxonomy

     array(
        'type' => 'taxonomy',
        'heading' => 'Categories',
        'taxonomy' => 'category',
        'param_name' => 'terms',
        ),
        
        
# Media field returns the id rather then the url

    array(
				'type' => 'media',
				'name' => 'upload',
				'label' => __('Image', 'ZX_TEXTDOMAIN'),
				'description' => __('mp4 recommended', 'ZX_TEXTDOMAIN'),
				'default' => 'http://placehold.it/70x70',
				);
				
More to come
