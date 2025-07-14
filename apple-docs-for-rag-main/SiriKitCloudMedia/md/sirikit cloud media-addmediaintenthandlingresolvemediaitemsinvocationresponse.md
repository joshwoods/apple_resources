

- SiriKit Cloud Media
-  AddMediaIntentHandlingResolveMediaItemsInvocationResponse 

Object

# AddMediaIntentHandlingResolveMediaItemsInvocationResponse

Your service’s response to a request to resolve media items in an update media affinity intent.

SiriKit Cloud Media 1.0.2+

``` source
object AddMediaIntentHandlingResolveMediaItemsInvocationResponse
```

## Properties

`result`

AddMediaIntentHandlingResolveMediaItemsInvocationResponse.Result

 (Required) 

The results of processing the intent.

`method`

`string`

 (Required) 

The action your service takes to process this intent.

Value: `AddMediaIntentHandling.resolveMediaItems`

## Topics

### Providing the Result

object AddMediaIntentHandlingResolveMediaItemsInvocationResponse.Result

The result of attempting to identify the media items to add to the user’s library or to a playlist.

## Relationships

### Inherits From

- InvocationResponse

## See Also

### Identifying a Media Item

object AddMediaMediaItemResolutionResult

A media item that matches an add media intent, or information about why your service can’t provide a media item.

