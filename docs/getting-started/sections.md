---
layout: docs
title: Adding Sections
edit: docs/getting-started/sections.md
---

Sections are wrappers for fields, a way to group multiple fields together. All fields must belong to a section, no field can be an orphan. To see how to create Sections using the WordPress Customizer API please take a look at [these docs](https://developer.wordpress.org/themes/advanced-topics/customizer-api/#sections).

```php
<?php
Kirki::add_section( 'section_id', array(
    'title'          => __( 'My title' ),
    'description'    => __( 'My descirption' ),
    'panel'          => '', // Not typically needed.
    'priority'       => 160,
    'capability'     => 'edit_theme_options',
    'theme_supports' => '', // Rarely needed.
) );
?>
```

The `Kirki::add_section()` method is nothing more than a wrapper for the WordPress customizer API and therefore follows the exact same syntax. More information on WordPress Customizer Sections can be found on the [WordPress Codex](https://developer.wordpress.org/themes/advanced-topics/customizer-api/#sections)
