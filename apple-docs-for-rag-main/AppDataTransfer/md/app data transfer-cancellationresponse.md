

- App Data Transfer
-  CancellationResponse 

Object

# CancellationResponse

An object that describes the outcome of canceling a download request.

App Data Transfer 1.0+

``` source
object CancellationResponse
```

## Properties

`jobStatus`

`string`

The current status of the download request.

Value: `cancelled`

`status`

`string`

The outcome of the cancellation operation.

Possible Values: `success, error`

## See Also

### Cancellation

Cancel request

Tells the server to stop processing an active request.

object CancellationRequest

An object that identifies a one-time request, or an individual instance of a recurring request, to cancel.

