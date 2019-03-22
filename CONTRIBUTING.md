# Contributing

Everyone is welcome to suggest an improvement to this resource. The goal is to make each point as clear as possible so reviews can move forward smoothly.

## New Issues

If you are contributing a new **Issue** then please try to follow this format.

1. Craft a clear title.
2. Explain the issue.
3. If an external resource that expands on the issue is available, provide a link.
4. Provide a code example if it helps.

### Example

#### Title:

Translation-Ready

#### Explanation:

All themes must be translatable-ready. This means users of any language can use your theme. To enable that you must use [WordPress' core translation functions] for all text. For example, in single.php on lines 5, 18 and 21 the text is not translatable.

#### Resource:

Resource: https://codex.wordpress.org/I18n_for_WordPress_Developers

#### Example:

`<?php esc_attr_e( 'Text to be translated', 'text-domain' ); ?>`
