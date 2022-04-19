# Maxmind GeoIP2 country buildpack for heroku `deprecated`

This buildpack will fetch the latest version of the GeoIP2 Country database upon deploy and install it in the desired location.

This package is intented to be used by those that have a active subscription/license with https://www.maxmind.com/en/geoip2-services-and-databases service.

## Requirements

This buildpack is designed to be used by node projects only, as such it has a few requirements that must be met before it may be used.

* You must have a package.json located in the root of your project containning the `@maxmind/geoip2-node` if not the buildpack will not activate and using it will change nothing.

* A valid license key and install path to be set in the env settings for your app prior to adding the builpack 

```
MAXMIND_GEOIP2_LICENSE_KEY=<The license key for your subscription on maxmind>

MAXMIND_GEOIP2_DB_PATH=<The relative path from the root of your project to the folder where the DB will be downloaded>
```

## Deprecated

This buildpack is no longer actively maintained, however it remains free to use, copy, fork etc.
