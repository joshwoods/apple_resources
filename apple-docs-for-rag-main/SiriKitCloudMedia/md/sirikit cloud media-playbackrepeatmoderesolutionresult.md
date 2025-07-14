

- SiriKit Cloud Media
-  PlaybackRepeatModeResolutionResult 

Object

# PlaybackRepeatModeResolutionResult

Information about whether your service can identify the specified repeat mode.

SiriKit Cloud Media 1.0.2+

``` source
object PlaybackRepeatModeResolutionResult
```

## Properties

`class`

`string`

The specific type of result.

Value: `PlaybackRepeatModeResolutionResult`

`success`

PlaybackRepeatModeResolutionResult.Success

A repeat mode that successfully matches the intent.

`confirmationRequired`

PlaybackRepeatModeResolutionResult.ConfirmationRequired

A repeat mode that the user must confirm or reject.

## Discussion

Only provide one of the optional properties. If a client receives a result with more than one outcome, such as `needsValue` and `success`, it arbitrarily chooses one and ignores the rest.

## Topics

### Specifying a Result

object PlaybackRepeatModeResolutionResult.Success

A playback mode that successfully matches the intent.

object PlaybackRepeatModeResolutionResult.ConfirmationRequired

A result that requires the user to confirm the playback mode before proceeding.

## Relationships

### Inherits From

- IntentResolutionResult

## See Also

### Resolving the Intended Repeat Mode

object PlayMediaIntentHandlingResolvePlaybackRepeatModeInvocationResponse

Your service’s response to a request to resolve the repeat mode in a play media intent.

object PlayMediaIntentHandlingResolvePlaybackRepeatModeInvocationResponse.Result

The result of resolving the repeat mode for a play media intent.

type PlaybackRepeatMode

The possible repeat modes for a media queue.

