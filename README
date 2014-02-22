## django-storages fork

s3boto backend claims: 

    # Dates returned from S3's API look something like this:
    "Sun, 11 Mar 2012 17:01:41 GMT"

when in fact I was getting something like this:

    "2014-02-22T06:34:26.000Z"

for last_modified datetime values on images uploaded to the Media Library.

This fork just updates the `DATESTR_RE` to properly parse the differing format
