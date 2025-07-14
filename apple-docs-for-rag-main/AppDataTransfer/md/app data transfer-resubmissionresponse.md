

- App Data Transfer
-  ResubmissionResponse 

Object

# ResubmissionResponse

An object that represents a resubmitted recurring download request.

App Data Transfer 1.0+

``` source
object ResubmissionResponse
```

## Properties

`parentRequestId`

`string`

A UUID that identifies the recurring request series.

`requestId`

`string`

A UUID that identifies the new request.

`status`

`string`

`success` if the server resubmitted the request; `error` otherwise.

`statusCheckDelay`

`integer`

The number of seconds to wait before you call Get recurring request status.

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

object ResubmissionRequest

An object that describes a request to resubmit a recurring download request.

