

- App Data Transfer
-  ResubmissionRequest 

Object

# ResubmissionRequest

An object that describes a request to resubmit a recurring download request.

App Data Transfer 1.0+

``` source
object ResubmissionRequest
```

## Properties

`parentRequestId`

`string`

A UUID that identifies the recurring request series.

`requestId`

`string`

A UUID that identifies the most recent download request in the recurring series.

## Overview

Use the `parentRequestId` and `requestId` returned by Submit request, or your most recent call to Resubmit request.

## See Also

### Request creation

Submit request

Starts preparing someone’s data for download.

object JobSubmission

An object that describes a submission that requests someone’s data.

object CreatedJob

An object that represents a newly created download request.

Resubmit request

Enqueue the next instance of a recurring request.

object ResubmissionResponse

An object that represents a resubmitted recurring download request.

