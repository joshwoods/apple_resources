

- App Data Transfer
-  DownloadError 

Object

# DownloadError

An object that describes an error the server encounters while preparing download URLs for a request.

App Data Transfer 1.0+

``` source
object DownloadError
```

## Properties

`statusCheckDelay`

`integer`

The number of seconds to wait before re-requesting the status.

`status`

`string`

The outcome of the operation.

Value: `error`

`statusMessage`

`string`

The reason the server encountered an error.

Possible Values: `in_progress, request_not_found, invalid_request_status`

## Overview

The `statusMessage` field has one of these values:

`invalid_request_status`  
The download request isn’t complete and you need to request the download URLs again after `statusCheckDelay` seconds.

`request_not_found`  
The request ID you provided isn’t recognized.

## See Also

### Downloads

Get one-time request download URLs

Get URLs to retrieve someone’s data.

Get recurring request download URLs

Get URLs to download a snapshot of someone’s data specific to your app from a recurring series.

object DownloadLinks

An object that contains URLs to download someone’s data specific to your app.

