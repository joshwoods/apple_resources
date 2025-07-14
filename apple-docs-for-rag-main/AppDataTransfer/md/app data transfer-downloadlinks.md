

- App Data Transfer
-  DownloadLinks 

Object

# DownloadLinks

An object that contains URLs to download someone’s data specific to your app.

App Data Transfer 1.0+

``` source
object DownloadLinks
```

## Properties

`assetInfo`

`[string]`

An array of URLs to which you make `GET` requests to download someone’s account data.

`jobStatus`

`string`

The result of the download request.

Possible Values: `completed, request_not_found, in_progress, error, completed_with_error, cancelled`

`status`

`string`

The result of the operation to request download links.

Value: `success`

## Overview

The URLs you get from the `assetInfo` property are valid for 15 minutes after you receive them.

## See Also

### Downloads

Get one-time request download URLs

Get URLs to retrieve someone’s data.

Get recurring request download URLs

Get URLs to download a snapshot of someone’s data specific to your app from a recurring series.

object DownloadError

An object that describes an error the server encounters while preparing download URLs for a request.

