# Installation of BHT Geolocation

## Composer requirements

This module is not available through a packagist which is why the requirements can not be defined a package specific
composer file. In order to successfully install the bht_geolocation module a few additional packages needs to be added
to the projects root composer file.

### Require the following packages withing the project
* drupal/geocoder
* drupal/geofield
* drupal/geofield_map
* drupal/leaflet
* geocoder-php/nominatim-provider

### Possible issues
Depending on the installed versions of the aforementioned packages it might be required to install a newer version of
the Guzzle package than what is required by Drupal. It might even be that the Guzzle version is fixed to a specific
version so that within the projects root composer file a newer version has to be defined masquerading as the other one.
The update of the package can be done as followed:
* "guzzlehttp/guzzle": "7.4.5 as 6.5.8"
