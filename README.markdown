[vimi.dk](http://vimi.dk) [![Build Status](https://secure.travis-ci.org/vimi/vimi-deploy.png?branch=7.x-1.x)](http://travis-ci.org/vimi/vimi-deploy)
==

Instructions on how to build the site from Drupal 7.

Requirements
------------

* [drush](http://drupal.org/project/drush) 
* [drush_make](http://drupal.org/project/drush_make)

Installation
------------

To build a complete site, run:

    drush make vimi_dk.build ~/workspace/vimi_dk_build

Navigate to the root directory in a webbrowser.

#### Update existing install profile ####

If you want to update just the install profile instead of rebuilding the
entire site, you can run this:

    drush make --no-core --contrib-destination=. vimi_dk.make

#### Rebuild everything ####

If you want to force a rebuild of everything, you can run this:

    drush si vimi_dk
