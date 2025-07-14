

- App Data Transfer
-  Get one-time request download URLs 

Web Service Endpoint

# Get one-time request download URLs

Get URLs to retrieve someone’s data.

App Data Transfer 1.0+

## URL

``` source
GET https://appdatatransfer.apple.com/api/transfer/appdata/fetch/{requestId}
```

## Path Parameters

`requestId`

`string`

 (Required) 

A UUID that identifies the one-time request.

## Response Codes

` 200 ``OK`

DownloadLinks

`OK`

Content-Type: application/json

` 400 ``Bad Request`

DownloadError

`Bad Request`

Content-Type: application/json

` 401 ``Unauthorized`

`Unauthorized`

` 403 ``Forbidden`

`Forbidden`

` 500 ``Internal Server Error`

`Internal Server Error`

## Overview

- Request
- Response

```
% curl -X GET \
  -H "Authorization: Bearer [ACCESS_TOKEN]" \
  -H "X-Apple-Transaction-Id: E3857B28-7FC4-41C8-AC54-08E121E26F59" \
  -H "X-Forwarded-For: 192.168.42.63" \
  -H "Accept: application/json" \
  https://appdatatransfer.apple.com/api/transfer/appdata/fetch/11619695-72C0-4FFD-858A-1E152DCF0838
```

```
{
  "assetInfo": [
    "https://assets.example.com/1.zip",
    "https://assets.example.com/2.zip"
  ],
  "jobStatus": "completed",
  "status": "success",
}
```

## See Also

### Downloads

Get recurring request download URLs

Get URLs to download a snapshot of someone’s data specific to your app from a recurring series.

object DownloadLinks

An object that contains URLs to download someone’s data specific to your app.

object DownloadError

An object that describes an error the server encounters while preparing download URLs for a request.

