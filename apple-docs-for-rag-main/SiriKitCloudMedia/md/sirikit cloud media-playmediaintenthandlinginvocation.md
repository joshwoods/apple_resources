

- SiriKit Cloud Media
-  PlayMediaIntentHandlingInvocation 

Object

# PlayMediaIntentHandlingInvocation

A request to process a play media intent.

SiriKit Cloud Media 1.0.2+

``` source
object PlayMediaIntentHandlingInvocation
```

## Properties

`params`

PlayMediaIntentHandlingInvocation.Params

 (Required) 

The parameters of this request, including the play media intent.

`method`

`string`

 (Required) 

The action for your service to take to process this intent.

Possible Values: `PlayMediaIntentHandling.resolveMediaItems, PlayMediaIntentHandling.resolvePlayShuffled, PlayMediaIntentHandling.resolvePlaybackQueueLocation, PlayMediaIntentHandling.resolvePlaybackRepeatMode, PlayMediaIntentHandling.resolveResumePlayback, PlayMediaIntentHandling.handle`

## Topics

### Accessing the Intent

object PlayMediaIntentHandlingInvocation.Params

The parameters of a play media intent request.

## Relationships

### Inherits From

- Invocation

## See Also

### Processing a Play Media Intent

object PlayMediaIntent

An object that describes the user’s request to play a media item.

type PlayMediaIntentHandlingInvocationResponse

The service’s response to a request to process a play media intent.

