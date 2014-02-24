## django-storages for Mezzanine deployed on Heroku with assets served from S3

s3boto.py backend claimed: 

    # Dates returned from S3's API look something like this:
    "Sun, 11 Mar 2012 17:01:41 GMT"

when in fact I was getting something like this:

    "2014-02-22T06:34:26.000Z"

for last_modified datetime values when uploading images to Mezzanine's Media Library.

This fork adds support for ISO8601 Extended and Basic formatted datetime strings
