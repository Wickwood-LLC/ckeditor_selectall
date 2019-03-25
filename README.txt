CKEditor Select All
--------------------------------------------------------------------------------

This plugin adds `Select All` functionality for CKEditor in Drupal 8:

- Quickly selects all the text.

INSTALLATION
------------

Manual
------
1. Download the plugin from http://ckeditor.com/addon/selectall.
2. Place the 'selectall' plugin directory within the root libraries folder in a
   (DRUPAL_ROOT/libraries/selectall).
3. Enable the CKEditor 'Select All' module.
4. Configure your WYSIWYG toolbar to include the buttons.

Composer
--------
1. Add the following repository to you composer.json file:

{
  "repositories": [
    {
      "type": "package",
      "package": {
        "name": "ckeditor/selectall",
        "version": "4.8.0",
        "type": "drupal-library",
        "extra": {
          "installer-name": "selectall"
        },
        "dist": {
          "url": "https://download.ckeditor.com/selectall/releases/selectall_4.8.0.zip",
          "type": "zip"
        }
      }
    }
  ]
}

2. Add the following installer-path to your composer file:

{
  "extra": {
    "installer-paths": {
      "libraries/{$name}": ["ckeditor/selectall"]
    }
  }
}
2.1 Run `composer require ckeditor/selectall 4.8.0`
3. Install and Enable the CKEditor `Select All` module.
4. Configure your WYSIWYG toolbar to include the buttons.
