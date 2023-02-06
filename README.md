# READ ME

This file needs to be in /ome/apache2/
with the name of your checkmk instance

# replace the following:
# [cmk.your-domain.com] with your domain name
# [your-site] with the name of your checkmk instance
# [ssl cert] with the path of your SSL certificates

# make sure to backup the existing config


This configuration file redirects http to https and the "/" path to the location of your Check_MK instance.

You need to change the following:
- "[ssl cert]" with the path of your SSL certificates
- "[your-site]" with the name of your checkmk instance
- "[cmk.your-domain.com]" with your domain name

Please make sure to backup the existing config.
After all this you need to reload the webserver using 'omd reload [your-site] apache'
