

- SiriKit Cloud Media
-  PlaybackQueueLocationResolutionResult 

Object

# PlaybackQueueLocationResolutionResult

Information about whether your service can resolve the specified queue location.

SiriKit Cloud Media 1.0.2+

``` source
object PlaybackQueueLocationResolutionResult
```

## Properties

`class`

`string`

The specific type of result.

Value: `PlaybackQueueLocationResolutionResult`

`success`

PlaybackQueueLocationResolutionResult.Success

A queue location that matches the intent.

`confirmationRequired`

PlaybackQueueLocationResolutionResult.ConfirmationRequired

A queue location for the user to confirm or reject before proceeding.

## Discussion

Only provide one of the optional properties. If a client receives a result with more than one outcome, such as `needsValue` and `success`, it arbitrarily chooses one and ignores the rest.

## Topics

### Specifying a Result

object PlaybackQueueLocationResolutionResult.Success

A queue location that matches the intent.

object PlaybackQueueLocationResolutionResult.ConfirmationRequired

A result that requires the user to confirm the playback mode before proceeding.

## Relationships

### Inherits From

- IntentResolutionResult

## See Also

### Resolving the Intended Queue Location

object PlayMediaIntentHandlingResolvePlaybackQueueLocationInvocationResponse

Your service’s response to a request to resolve the queue location in a play media intent.

type PlaybackQueueLocation

Possible locations in a playback queue to insert a media item.

