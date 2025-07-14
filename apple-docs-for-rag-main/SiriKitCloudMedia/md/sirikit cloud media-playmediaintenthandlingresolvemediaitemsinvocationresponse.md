

- SiriKit Cloud Media
-  PlayMediaIntentHandlingResolveMediaItemsInvocationResponse 

Object

# PlayMediaIntentHandlingResolveMediaItemsInvocationResponse

Your service’s response to a request to resolve media items in a play media intent.

SiriKit Cloud Media 1.0.2+

``` source
object PlayMediaIntentHandlingResolveMediaItemsInvocationResponse
```

## Properties

`result`

PlayMediaIntentHandlingResolveMediaItemsInvocationResponse.Result

 (Required) 

The results of processing the intent.

`method`

`string`

 (Required) 

The action your service takes to process this intent.

Value: `PlayMediaIntentHandling.resolveMediaItems`

## Topics

### Specifying the Result

object PlayMediaIntentHandlingResolveMediaItemsInvocationResponse.Result

The results of resolving the media items in an intent to play media.

## Relationships

### Inherits From

- InvocationResponse

## See Also

### Resolving a Media Item

object PlayMediaMediaItemResolutionResult

A media item that matches a play media intent, or information about why your service can’t provide a media item.

type PlayMediaMediaItemUnsupportedReason

Reasons the media service can’t play the media item.

