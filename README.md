![geniem-github-banner](https://cloud.githubusercontent.com/assets/5691777/14319886/9ae46166-fc1b-11e5-9630-d60aa3dc4f9e.png)
# WordPress Plugin Collection for Search Engine Optimizations
[![Latest Stable Version](https://poser.pugx.org/devgeniem/wp-seo-collection/v/stable)](https://packagist.org/packages/devgeniem/wp-seo-collection) [![Total Downloads](https://poser.pugx.org/devgeniem/wp-seo-collection/downloads)](https://packagist.org/packages/devgeniem/wp-seo-collection) [![Latest Unstable Version](https://poser.pugx.org/devgeniem/wp-seo-collection/v/unstable)](https://packagist.org/packages/devgeniem/wp-seo-collection) [![License](https://poser.pugx.org/devgeniem/wp-seo-collection/license)](https://packagist.org/packages/devgeniem/wp-seo-collection)

This is WordPress plugin and dropin collection which enables search engine optimizations.

## Reasons
This package was created to handle multiple projects with `composer update`. We just include this collection into our `composer.json` and stick to the guidelines about which plugins should be included here. WordPress evolves with time and some plugins will propably be pointless at some point, if that happens we will remove those unneccessary plugins.

## Installation
```
$ composer require devgeniem/wp-seo-collection
```

## Requirements
* >= PHP 7.0
* WordPress
* Use composer to update your site rather than using WordPress auto updates

### Composer.json settings
For correct installation your project should define following installation paths in `extra` section:
```
extra: {
    "installer-paths": {
      "web/app/mu-plugins/{$name}/": ["type:wordpress-muplugin"],
      "web/app/plugins/{$name}/": ["type:wordpress-plugin"]
    },
    "dropin-paths": {
      "web/app/": ["type:wordpress-dropin"]
    }
}
```

We use bedrock styled names for `wp-content`. Replace `web/app` according for your project.

## Maintainers
[Ville Siltala](https://github.com/villesiltala)

## Changelog
[See the included CHANGELOG.md](CHANGELOG.md)

## License
Respect the licenses of used libraries. This readme and composer are licensed under MIT
