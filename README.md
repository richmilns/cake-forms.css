cake-forms.css
==============

![Cake Forms Example](http://i40.tinypic.com/2llzibt.jpg)

A plugin for CakePHP 2.x which provides base CSS styles for forms created using the FormHelper. 

The code has been written using LESS and can be totally customised to your requirements by altering the variables at the top of the cake-forms.less file and recompiling.

Styles have been created for:
- Forms of different widths (you can apply classes like cake-form-width-75 for 75% for example)
- Inline forms (for example login forms)
- 'Horizontal' forms with the label to the left of the form elements

The code less than 4kb (gzipped). The CSS version is already minified. Please note that inline and horizontal styles only work in IE9+ (they require CSS media query support).

Handy features:
- Automatically makes your CakePHP forms responsive out of the box!
- Provides an elegant baseline style for rapid prototyping
- Doesn't interfere with other existing form styles
- Support for IE7+ (looks OK on IE6 too)

Feel free to make any suggestions or file a bug if you spot anything and I'll do my best to look into them in future releases.

Installation
============
1. Clone into your project's `Plugin` folder
2. Load the plugin from your bootstrap.php: `CakePlugin::load('CakeForms');`
3. Add to your layout's head: `echo $this->Html->css('/cake_forms/css/cake-forms');`
4. Add the class `cake-form` to any form and voila!
5. Play around with adding additional classes such as `cake-form-inline` or `cake-form-horizontal` or `cake-form-width-50` (see the LESS file for more widths)

If you are using the LESS version, you will also need to download the following into your less folder:
- LessHat2 (https://github.com/csshat/lesshat/)
- Remixins (https://github.com/christopher-ramirez/remixings)

Future Ideas
============
- I'm looking to implement a grid system to allow forms to be created in columns
- More responsive CSS
- Better support for IE7/8 - e.g. horizontal & inline forms 

Version History
===============
**1.0.0** - first release
