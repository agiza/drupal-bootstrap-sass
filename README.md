#Drupal Boostrap Sub-Theme (SASS)
This is a sub-theme for the [Drupal Bootstrap theme](https://drupal.org/project/bootstrap). Instead of using less / css, this uses SASS. It's also been setup to use local CSS / JS files by default, this is because the entire Bootstrap CSS is generated by SASS.

##Pre-requisists
1. Install compass:

		gem install compass
2. Install bootstrap-sass

		gem install bootstrap-sass
		
##Using the theme
Either use drush to download the boostrap theme:

``drush dl bootstrap``

Or manually download and add to ``sites/all/themes`` (or your current site themes folder).

Download this basetheme and add to your themes folder.

Rename the folder to ``you-theme-name``

Rename ``drupal-bootstrap-base.info.starterkit`` to ``your-theme-name.info``

In ``config.rb`` change the http_path to path to your theme. This is the URL visitors use to access your theme. e.g. a standard URL would be ``/sites/default/themes/my-theme/``

Ok, compass should now be able to compile your theme:

``cd path-to-your-theme``

``compass compile``

Or you can watch for chanages with

``compass watch``

You can now enable the theme in Drupal.

##Customising the theme
Your first port of call should be the ``_variables.scss`` partial. These are all the variables used by bootstrap. To change something, just uncomment the variable and change to your value.

Your own styles should go in the ``_custom.scss`` partial. You can use all the bootstrap variables and mixins, along with all the compass functions / mixins.

If you need to tweak some templates - copy them over from the bootstrap parent theme. Place them into the templates folder.

##Contributing
PR are welcome and appriciated - if you are unsure or have any questions get in touch or let us know on [Twitter](http://www.twitter/Arrow_UK).

Built by [Arrow](http://www.arrowdesign.co.uk/)