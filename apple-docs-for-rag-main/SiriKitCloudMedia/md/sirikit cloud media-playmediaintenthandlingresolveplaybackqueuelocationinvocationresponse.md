

- SiriKit Cloud Media
-  PlayMediaIntentHandlingResolvePlaybackQueueLocationInvocationResponse 

Object

# PlayMediaIntentHandlingResolvePlaybackQueueLocationInvocationResponse

Your service’s response to a request to resolve the queue location in a play media intent.

SiriKit Cloud Media 1.0.2+

``` source
object PlayMediaIntentHandlingResolvePlaybackQueueLocationInvocationResponse
```

## Properties

`result`

PlayMediaIntentHandlingResolvePlaybackQueueLocationInvocationResponse.Result

 (Required) 

The result of processing the intent.

`method`

`string`

 (Required) 

The action your service takes to process this intent.

Value: `PlayMediaIntentHandling.resolvePlaybackQueueLocation`

## Topics

### Specifying a Result

object PlayMediaIntentHandlingResolvePlaybackQueueLocationInvocationResponse.Result

The result of resolving the queue location for a play media intent.

## Relationships

### Inherits From

- InvocationResponse

## See Also

### Resolving the Intended Queue Location

object PlaybackQueueLocationResolutionResult

Information about whether your service can resolve the specified queue location.

type PlaybackQueueLocation

Possible locations in a playback queue to insert a media item.

