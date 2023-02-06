# READ ME FIRST

The file needs to be in `/omd/apache/` with the name of your isntance


This configuration file redirects http to https and the "/" path to the location of your Check_MK instance.

You need to change the following:
- "[ssl cert]" with the path of your SSL certificates
- "[your-site]" with the name of your checkmk instance
- "[cmk.your-domain.com]" with your domain name

Please make sure to backup the existing config.
After all this you need to reload the webserver using 'omd reload [your-site] `apache`
