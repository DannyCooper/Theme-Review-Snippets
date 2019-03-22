# Table of Contents  

**[Review Template](#review-template)**<br>
**[Issues](#issues)**<br>

## Review Template

Hi @user,

I will be reviewing your theme today. The theme review process includes manually checking each file, as well as testing your theme using the 'Theme Sniffer' plugin. Using this tool in your development process may help with approval.

https://wordpress.org/plugins/theme-sniffer/

There are standards required of themes before they can be accepted into the WordPress.org directory, those can be found here - https://make.wordpress.org/themes/handbook/review/required/

If your theme does not comply with 3 or more of those requirements, this ticket will be closed and the theme resolved as not-approved.

Once you have fixed the issues, the theme can be re-uploading using a higher version number in style.css. However, it will join the back of the review queue.

**== Issues**

*Issues go here.*

**== Further Information**

For discussion regarding the theme review process, we have an active Slack Channel https://wordpress.slack.com/messages/themereview/

---

## Issues

#### '''Licensing

Every resource included with your theme that you didn't create should be GPL-compatible. Also, the license information should be easily accessible within readme.txt. Resources include:
```
1. Images
2. Scripts
3. Libraries
4. Frameworks
5. Fonts
6. Icons
```

The preferred format for documenting each resource is the following:

`> Resource Name - Resource URL - License - License URL`

For example:

`> FontAwesome - http://fontawesome.io - MIT License - http://fontawesome.io/license`

#### '''Theme URI

The Theme URI is optional. But if it's used, it must be about the theme we’re hosting on WordPress.org. Not a theme demo.

#### '''Translation-Ready

All themes must be translatable-ready. This means users of any language can use your theme. To enable that you must use [WordPress' core translation functions] for all text. For example, in single.php on lines 5, 18 and 21 the text is not translatable.

Resource: https://codex.wordpress.org/I18n_for_WordPress_Developers

#### '''readme.txt

Your theme readme.txt must follow this format - https://make.wordpress.org/themes/2015/04/29/a-revised-readme/

In the future, the WordPress.org directory will pull information about your theme from the readme.txt, so it's important to enforce a standard format. 

There is a readme.txt validator:

https://wordpress.org/plugins/developers/readme-validator/ 

Your readme.txt should return no **Warnings:**

#### '''Third-Party Enqueue Handles

Themes must not use a prefix for third-party resources. 

Some themes and plugins rely on the same third-party scripts and styles. By using a standard handle we can ensure they aren't loaded twice or more. 

**''Correct''**

    > wp_enqueue_script( 'modernizr', get_template_directory_uri() . '/js/modernizr.js', array('jquery') );
    
**''Incorrect''**

    > wp_enqueue_script( 'mytheme-modernizr', get_template_directory_uri() . '/js/modernizr.js', array('jquery') );

Files are empty or contain only commented out code should be removed as they provide no value to the user.

#### '''Empty Files and Folders

Files are empty or contain only commented out code should be removed as they provide no value to the user.

#### '''Open Graph Meta Tags (Facebook, Twitter, etc.)

This is considered plugin-territory and should not be included within a theme. There are a lot of popular plugins that output this data.
