

- SiriKit Cloud Media
-  UpdateMediaAffinityIntentHandlingResolveMediaItemsInvocationResponse 

Object

# UpdateMediaAffinityIntentHandlingResolveMediaItemsInvocationResponse

Your service’s response to a request to resolve media items in an update media affinity intent.

SiriKit Cloud Media 1.0.2+

``` source
object UpdateMediaAffinityIntentHandlingResolveMediaItemsInvocationResponse
```

## Properties

`method`

`string`

 (Required) 

The results of processing the intent.

Value: `UpdateMediaAffinityIntentHandling.resolveMediaItems`

`result`

UpdateMediaAffinityIntentHandlingResolveMediaItemsInvocationResponse.Result

 (Required) 

The action your service takes to process this intent.

## Topics

### Specifying the Result

object UpdateMediaAffinityIntentHandlingResolveMediaItemsInvocationResponse.Result

The results of resolving the media items in an intent to update media affinity.

## Relationships

### Inherits From

- InvocationResponse

## See Also

### Identifying the Intended Media Items

object UpdateMediaAffinityMediaItemResolutionResult

A media item that matches an update media affinity intent, or information about why your service can’t provide a media item.

type UpdateMediaAffinityMediaItemUnsupportedReason

Reasons the media service can’t update information about the media item.

