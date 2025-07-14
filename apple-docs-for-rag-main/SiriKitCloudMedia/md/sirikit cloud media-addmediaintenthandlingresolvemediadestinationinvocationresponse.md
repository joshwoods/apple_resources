

- SiriKit Cloud Media
-  AddMediaIntentHandlingResolveMediaDestinationInvocationResponse 

Object

# AddMediaIntentHandlingResolveMediaDestinationInvocationResponse

Your service’s response to a request to resolve media items in an add media intent.

SiriKit Cloud Media 1.0.2+

``` source
object AddMediaIntentHandlingResolveMediaDestinationInvocationResponse
```

## Properties

`result`

AddMediaIntentHandlingResolveMediaDestinationInvocationResponse.Result

 (Required) 

The results of processing the intent.

`method`

`string`

 (Required) 

The action your service takes to process this intent.

Value: `AddMediaIntentHandling.resolveMediaDestination`

## Topics

### Specifying the Result

object AddMediaIntentHandlingResolveMediaDestinationInvocationResponse.Result

The result of attempting to modify the user’s library or a playlist.

## Relationships

### Inherits From

- InvocationResponse

## See Also

### Identifying a Library or Playlist

object AddMediaMediaDestinationResolutionResult

The user’s library or a specified playlist, or information about why your service can’t use the requested destination.

