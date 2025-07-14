

- Account Data Transfer
-  Submit request 

Web Service Endpoint

# Submit request

Starts preparing someone’s data for download.

Account Data Transfer 1.0+

## URL

``` source
POST https://accountdatatransfer.apple.com/api/transfer/accountdata/submit
```

## HTTP Body

JobSubmission

The description of the new download request.

Content-Type: application/json

## Response Codes

` 200 ``OK`

CreatedJob

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

Request the `app-store` data type to get App Store information and app-install activity.

### Request a one-time download

- Request
- Response

```
% curl -X POST \
  -H "Authorization: Bearer [ACCESS_TOKEN]" \
  -H "X-Apple-Transaction-Id: E3857B28-7FC4-41C8-AC54-08E121E26F59" \
  -H "X-Forwarded-For: 192.168.42.63" \
  -H "Content-Type: application/json" \
  -d '{ "mode": "ONE_TIME" }' \
  https://accountdatatransfer.apple.com/api/transfer/accountdata/submit
```

```
{
  "requestId": "11619695-72C0-4FFD-858A-1E152DCF0838",
  "status": "in_progress",
  "statusCheckDelay": 86400
}
```

### Request a recurring download

- Request
- Response

```
% curl -X POST \
  -H "Authorization: Bearer [ACCESS_TOKEN]" \
  -H "X-Apple-Transaction-Id: E3857B28-7FC4-41C8-AC54-08E121E26F59" \
  -H "X-Forwarded-For: 192.168.42.63" \
  -H "Content-Type: application/json" \
  -d '{ "mode": "DAILY_30" }' \
  https://accountdatatransfer.apple.com/api/transfer/accountdata/submit
```

```
{
  "parentRequestId": "EABD06C0-9210-47FF-83C4-318CF8520644",
  "requestId": "7BBBD45D-638B-4DB5-8B02-F23FDB15EDA7",
  "status": "in_progress",
  "statusCheckDelay": 86400
}
```

## See Also

### Request creation

object JobSubmission

An object that describes a submission that requests someone’s data.

object CreatedJob

An object that represents a newly created download request.

Resubmit request

Enqueue the next instance of a recurring request.

object ResubmissionRequest

An object that describes a request to resubmit a recurring download request.

object ResubmissionResponse

An object that represents a resubmitted recurring download request.

