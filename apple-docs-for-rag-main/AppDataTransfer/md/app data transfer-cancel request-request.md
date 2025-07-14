

- App Data Transfer
-  Cancel request 

Web Service Endpoint

# Cancel request

Tells the server to stop processing an active request.

App Data Transfer 1.0+

## URL

``` source
POST https://appdatatransfer.apple.com/api/transfer/appdata/cancel
```

## HTTP Body

CancellationRequest

An object that identifies the request to cancel.

Content-Type: application/json

## Response Codes

` 200 ``OK`

CancellationResponse

`OK`

Content-Type: application/json

` 400 ``Bad Request`

`Bad Request`

` 401 ``Unauthorized`

`Unauthorized`

` 403 ``Forbidden`

`Forbidden`

` 500 ``Internal Server Error`

`Internal Server Error`

## Overview

A cancellation request only succeeds if the request is currently in progress.

### Cancel a one-time download

- Request
- Response

```
% curl -X POST \
  -H "Authorization: Bearer [ACCESS_TOKEN]" \
  -H "X-Apple-Transaction-Id: E3857B28-7FC4-41C8-AC54-08E121E26F59" \
  -H "X-Forwarded-For: 192.168.42.63" \
  -H "Content-Type: application/json" \
  -d '{ "requestId": "11619695-72C0-4FFD-858A-1E152DCF0838" }' \
  https://appdatatransfer.apple.com/api/transfer/appdata/cancel
```

```
{
  "jobStatus": "cancelled",
  "status": "success"
}
```

### Cancel a recurring download

- Request
- Response

```
% curl -X POST \
  -H "Authorization: Bearer [ACCESS_TOKEN]" \
  -H "X-Apple-Transaction-Id: E3857B28-7FC4-41C8-AC54-08E121E26F59" \
  -H "X-Forwarded-For: 192.168.42.63" \
  -H "Content-Type: application/json" \
  -d '{ "requestId": "7BBBD45D-638B-4DB5-8B02-F23FDB15EDA7-parentEABD06C0-9210-47FF-83C4-318CF8520644" }' \
  https://appdatatransfer.apple.com/api/transfer/appdata/cancel
```

```
{
  "jobStatus": "cancelled",
  "status": "success"
}
```

## See Also

### Cancellation

object CancellationRequest

An object that identifies a one-time request, or an individual instance of a recurring request, to cancel.

object CancellationResponse

An object that describes the outcome of canceling a download request.

