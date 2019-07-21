# Errors

The Item API uses the following error codes:


Error Code | Meaning
---------- | -------
400 | Bad Request -- Your request is invalid.
401 | Unauthorized -- Your Token is wrong.
403 | Forbidden -- The item requested is hidden for administrators only.
404 | Not Found -- The specified item could not be found.
405 | Method Not Allowed -- You tried to access a item with an invalid method.
429 | Too Many Requests -- You're requesting too many item! Slow down!
500 | Internal Server Error -- We had a problem with our server. Try again later.
503 | Service Unavailable -- We're temporarily offline for maintenance. Please try again later.
