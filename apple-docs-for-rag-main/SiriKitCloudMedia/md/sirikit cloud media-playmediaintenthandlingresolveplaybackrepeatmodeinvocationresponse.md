

- SiriKit Cloud Media
-  PlayMediaIntentHandlingResolvePlaybackRepeatModeInvocationResponse 

Object

# PlayMediaIntentHandlingResolvePlaybackRepeatModeInvocationResponse

Your service’s response to a request to resolve the repeat mode in a play media intent.

SiriKit Cloud Media 1.0.2+

``` source
object PlayMediaIntentHandlingResolvePlaybackRepeatModeInvocationResponse
```

## Properties

`result`

PlayMediaIntentHandlingResolvePlaybackRepeatModeInvocationResponse.Result

 (Required) 

The result of processing the intent.

`method`

`string`

 (Required) 

The action your service takes to process this intent.

Value: `PlayMediaIntentHandling.resolvePlaybackRepeatMode`

## Topics

### Specifying a Result

object PlayMediaIntentHandlingResolvePlaybackRepeatModeInvocationResponse.Result

The result of resolving the repeat mode for a play media intent.

## Relationships

### Inherits From

- InvocationResponse

## See Also

### Resolving the Intended Repeat Mode

object PlayMediaIntentHandlingResolvePlaybackRepeatModeInvocationResponse.Result

The result of resolving the repeat mode for a play media intent.

object PlaybackRepeatModeResolutionResult

Information about whether your service can identify the specified repeat mode.

type PlaybackRepeatMode

The possible repeat modes for a media queue.

