

- Account Data Transfer
-  RequestStatus 

Object

# RequestStatus

An object that represents the status of a download request.

Account Data Transfer 1.0+

``` source
object RequestStatus
```

## Properties

`jobStatus`

`string`

The status of the download request.

Possible Values: `completed, request_not_found, in_progress, error, completed_with_error, cancelled`

`status`

`string`

`success` if the operation succeeded; `error` otherwise.

`statusCheckDelay`

`integer`

The number of seconds to wait before re-requesting the status.

## See Also

### Status

Get one-time request status

Find the status of a one-time download request.

Get recurring request status

Get the status of an instance of a recurring download request.

