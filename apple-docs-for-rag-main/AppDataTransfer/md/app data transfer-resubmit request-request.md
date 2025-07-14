

- App Data Transfer
-  Resubmit request 

Web Service Endpoint

# Resubmit request

Enqueue the next instance of a recurring request.

App Data Transfer 1.0+

## URL

``` source
POST https://appdatatransfer.apple.com/api/transfer/appdata/resubmit
```

## HTTP Body

ResubmissionRequest

The recurring request for which you submit a new instance.

Content-Type: application/json

## Response Codes

` 200 ``OK`

ResubmissionResponse

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

The `requestId` you pass must be the most recent instance of the series identified by the `parentRequestId`.

- Request
- Response

```
% curl -X POST \
  -H "Authorization: Bearer [ACCESS_TOKEN]" \
  -H "X-Apple-Transaction-Id: E3857B28-7FC4-41C8-AC54-08E121E26F59" \
  -H "X-Forwarded-For: 192.168.42.63" \
  -H "Content-Type: application/json" \
  -d '{ "parentRequestId": "EABD06C0-9210-47FF-83C4-318CF8520644", "requestId": "7BBBD45D-638B-4DB5-8B02-F23FDB15EDA7" }' \
  https://appdatatransfer.apple.com/api/transfer/appdata/resubmit
```

```
{
  "parentRequestId": "EABD06C0-9210-47FF-83C4-318CF8520644",
  "requestId": "A2DFE115-F039-4FC4-8286-7EAD51D91D8B",
  "status": "completed",
  "statusCheckDelay": 86400
}
```

## See Also

### Request creation

Submit request

Starts preparing someone’s data for download.

object JobSubmission

An object that describes a submission that requests someone’s data.

object CreatedJob

An object that represents a newly created download request.

object ResubmissionRequest

An object that describes a request to resubmit a recurring download request.

object ResubmissionResponse

An object that represents a resubmitted recurring download request.

