

- App Data Transfer
-  CancellationRequest 

Object

# CancellationRequest

An object that identifies a one-time request, or an individual instance of a recurring request, to cancel.

App Data Transfer 1.0+

``` source
object CancellationRequest
```

## Properties

`requestId`

`string`

An identifier for the request to cancel. For a one-time request, use the request’s UUID. For a recurring request, combine the request and parent UUIDs in this format: `[requestId]-parent[parentRequestID]`.

## See Also

### Cancellation

Cancel request

Tells the server to stop processing an active request.

object CancellationResponse

An object that describes the outcome of canceling a download request.

