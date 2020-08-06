# Maxmind GeoIP2 country buildpack for heroku

This buildpack will fetch the latest version of the GeoIP2 Country database upon deploy and install it in the desired location

To use you must first add the following config values to your heroku env settings

`MAXMIND_GEOIP2_LICENSE_KEY`: The license key for your subscription on maxmind

`MAXMIND_GEOIP2_DB_PATH`: The relative path from the root of your project to the folder where the DB will be downloaded
