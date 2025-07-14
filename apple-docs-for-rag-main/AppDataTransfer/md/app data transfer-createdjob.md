

- App Data Transfer
-  CreatedJob 

Object

# CreatedJob

An object that represents a newly created download request.

App Data Transfer 1.0+

``` source
object CreatedJob
```

## Properties

`parentRequestId`

`string`

For recurring requests, a UUID that identifies the series of requests. For one-time requests, the server doesn’t include this key in the response.

`requestId`

`string`

A UUID that identifies this request.

`status`

`string`

`completed` if the server created the request; `error` otherwise.

`statusCheckDelay`

`integer`

The number of seconds to wait before you call Get recurring request status or Get one-time request status.

## See Also

### Request creation

Submit request

Starts preparing someone’s data for download.

object JobSubmission

An object that describes a submission that requests someone’s data.

Resubmit request

Enqueue the next instance of a recurring request.

object ResubmissionRequest

An object that describes a request to resubmit a recurring download request.

object ResubmissionResponse

An object that represents a resubmitted recurring download request.

