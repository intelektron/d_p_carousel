# Slick paragraph for Droopler #
[![N|Solid](http://intelektron.pl/logo.svg)](http://intelektron.pl)

## How does it look? ##

[![N|Solid](http://intelektron.pl/static/intelektron-slick-1.png)](http://intelektron.pl/static/intelektron-slick-1.png)

[![N|Solid](http://intelektron.pl/static/intelektron-slick-2.png)](http://intelektron.pl/static/intelektron-slick-2.png)

## Installation ##

1. Update **composer.json**

Put this module in the "require" section of your composer.json. I assume you have configured asset-packagist.org and "composer-installers-extender" extension.

```json
"require": {
  "intelektron/d_p_carousel":  "^1.0",
  "npm-asset/slick-carousel": "^1.8"
}
```

In the "repositories" section put:

```json
"repositories": {
  "intelektron-carousel": {
    "type": "git",
    "url":  "git@github.com:intelektron/d_p_carousel.git"
  }
}
```

2. Run **composer update**.
3. Include module's scss in droopler_subtheme style.scss file

```scss
@import "../../../../modules/contrib/d_p_carousel/scss/d_p_carousel";
```

**Note**: Any changes made in this file won't be caught by **gulp watch**.

4. Run **gulp compile** in droopler_subtheme directory
5. Enable module in Drupal.
6. Enjoy the new paragraph :-).
