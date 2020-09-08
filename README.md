# Timezone Detect

Timezone Detect is a lightweight Backdrop module that leverages the 
`jsTimezoneDetect` library (bundled with the module) for automatic detection and 
setting of a user's timezone via Javascript. It can set a user's timezone 
automatically upon first login, and update it on every login if desired.

## Installation and Configuration

- Install this module using the [official Backdrop CMS instructions](https://backdropcms.org/guide/modules).

This module is designed to be "set it and forget it": it does not require any 
special installation or configuration beyond enabling the module. It defaults to 
setting a user's timezone automatically at login if their timezone is not yet 
set.

If desired, there are a couple of options that can be configured by visiting 
**admin/config/regional/timezone_detect**.

When using this module it is recommended that you disable the option to "Remind 
users at login if their time zone is not set" in Backdrop's regional settings, by 
visiting **admin/config/regional/settings** and unchecking that option. Otherwise 
users may be asked to set their timezone on first login even when this module 
has already set it via AJAX callback. This setting is disabled automatically 
when Timezone Detect is first enabled.

## Documentation

More details may be found (or contributed to) in the [Wiki](https://github.com/backdrop-contrib/timezone_detect/wiki).

## Issues

Bugs and Feature requests should be reported in the [Issue Queue](https://github.com/backdrop-contrib/timezone_detect/issues)

# Current Maintainers

- [Laryn Kragt Bakker](https://github.com/laryn), [CEDC.org](https://CEDC.org)
- Collaboration and co-maintainers welcome!

## Credits

- Ported to Backdrop by [Laryn Kragt Bakker](https://github.com/laryn), [CEDC.org](https://CEDC.org)
- Written and maintained for Drupal by [Jordan Magnuson](https://drupal.org/user/269983)

## License

This project is GPL v2 software. See the LICENSE.txt file in this directory for
complete text.

The `jsTimezoneDetect` library is released under the MIT license.
