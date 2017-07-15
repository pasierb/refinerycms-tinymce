# TinyMCE Visual Editing for RefineryCMS

TinyMCE is a platform independent web based Javascript HTML WYSIWYG editor control released as Open Source under LGPL.

This is an extention to Refinery to use TinyMCE as the editor in text fields.

This fork of original work by ghoppe https://github.com/ghoppe/refinerycms-tinymce that provides
TinyCMS from CDN. It works out of the box, but you may want to register your copy to get rid of "API Key" notification.
Once you obtain api key put it into secrets.yml

```
production:
  tinymce_spi_key: YOUR_API_KEY
```


![](http://img-fotki.yandex.ru/get/94893/203537249.14/0_151ef7_7145b111_orig.png)



## Installation

Replace in Gemfile:
```
gem 'refinerycms-wymeditor', ['~> 1.0', '>= 1.0.6']
```
with:
```
gem 'refinerycms-tinymce', git: 'https://github.com/pasierb/refinerycms-tinymce'
```
And run:
```
bundle install
```
Restart server.

## Customization

TODO

## Dialogs that show from TinyMCE

### Page Link dialog

The link dialog lets you link in several different ways:

* To an internal page
* To an external page
* To an email address
* To a resource you've uploaded in the Resources tab.

### Insert Image dialog

Simply lets you select from an existing image found in the Images tab or upload
a new one right within the dialog.
