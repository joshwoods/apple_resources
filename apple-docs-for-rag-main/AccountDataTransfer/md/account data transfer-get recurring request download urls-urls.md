

- Account Data Transfer
-  Get recurring request download URLs 

Web Service Endpoint

# Get recurring request download URLs

Get URLs to download a snapshot of someone’s data from a recurring series.

Account Data Transfer 1.0+

## URL

``` source
GET https://accountdatatransfer.apple.com/api/transfer/accountdata/fetch/{parentRequestId}/{requestId}
```

## Path Parameters

`requestId`

`string`

 (Required) 

A UUID that identifies the individual download request in the recurring sequence.

`parentRequestId`

`string`

 (Required) 

A UUID that identifies the recurring sequence of download requests.

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
  https://accountdatatransfer.apple.com/api/transfer/accountdata/fetch/EABD06C0-9210-47FF-83C4-318CF8520644/7BBBD45D-638B-4DB5-8B02-F23FDB15EDA7
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

Get one-time request download URLs

Get URLs to retrieve someone’s data.

object DownloadLinks

An object that contains URLs to download someone’s account data.

object DownloadError

An object that describes an error the server encounters preparing download URLs for a request.

