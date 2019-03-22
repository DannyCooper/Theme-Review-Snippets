## Review Template

Hi @user,

I will be reviewing your theme today. There are standards required of themes before they can be accepted into the WordPress.org directory, those can be found here - https://make.wordpress.org/themes/handbook/review/required/

If your theme does not comply with 3 or more of those requirements, this ticket will be closed and the theme resolved as not-approved.

Once you have fixed the issues, the theme can be re-uploading using a higher version number in style.css. However, it will join the back of the review queue.

**== Issues**

*Issues go here.*

**== Further Information**

For discussion regarding the theme review process, we have an active Slack Channel https://wordpress.slack.com/messages/themereview/

## Issues

**'''Theme URI**

The Theme URI is optional. But if it's used, it must be about the theme we’re hosting on WordPress.org. Not a theme demo.

**'''Translation-Ready**

All themes must be translatable-ready. This means users of any language can use your theme. To enable that you must use [WordPress' core translation functions] for all text. For example, in single.php on lines 5, 18 and 21 the text is not translatable.

Resource: https://codex.wordpress.org/I18n_for_WordPress_Developers

**'''readme.txt**

Your theme readme.txt must follow this format - https://make.wordpress.org/themes/2015/04/29/a-revised-readme/

In the future, the WordPress.org directory will pull information about your theme from the readme.txt, so it's important to enforce a standard format. 

There is a readme.txt validator:

https://wordpress.org/plugins/developers/readme-validator/ 

Your readme.txt should return no **Warnings:**
