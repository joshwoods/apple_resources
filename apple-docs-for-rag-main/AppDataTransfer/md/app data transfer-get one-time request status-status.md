

- App Data Transfer
-  Get one-time request status 

Web Service Endpoint

# Get one-time request status

Find the status of a one-time download request.

App Data Transfer 1.0+

## URL

``` source
GET https://appdatatransfer.apple.com/api/transfer/appdata/{requestId}
```

## Path Parameters

`requestId`

`string`

 (Required) 

A UUID that identifies the download request.

## Response Codes

` 200 ``OK`

RequestStatus

`OK`

Content-Type: application/json

## Overview

- Request
- Response

```
% curl -X GET \
  -H "Authorization: Bearer [ACCESS_TOKEN]" \
  -H "X-Apple-Transaction-Id: E3857B28-7FC4-41C8-AC54-08E121E26F59" \
  -H "X-Forwarded-For: 192.168.42.63" \
  -H "Accept: application/json" \
  https://appdatatransfer.apple.com/api/transfer/appdata/11619695-72C0-4FFD-858A-1E152DCF0838
```

```
{
  "jobStatus": "in_progress",
  "status": "success",
  "statusCheckDelay": 86400
}
```

## See Also

### Status

Get recurring request status

Get the status of an instance of a recurring download request.

object RequestStatus

An object that represents the status of a download request.

