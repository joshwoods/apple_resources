

- SiriKit Cloud Media
-  PlayMediaIntentHandlingResolveResumePlaybackInvocationResponse 

Object

# PlayMediaIntentHandlingResolveResumePlaybackInvocationResponse

Your service’s response to a request to resolve whether a play media intent resumes the current playback queue.

SiriKit Cloud Media 1.0.2+

``` source
object PlayMediaIntentHandlingResolveResumePlaybackInvocationResponse
```

## Properties

`result`

PlayMediaIntentHandlingResolveResumePlaybackInvocationResponse.Result

 (Required) 

The result of processing the intent.

`method`

`string`

 (Required) 

The action your service takes to process this intent.

Value: `PlayMediaIntentHandling.resolveResumePlayback`

## Topics

### Specifying a Result

object PlayMediaIntentHandlingResolveResumePlaybackInvocationResponse.Result

The result of resolving whether a play media intent resumes the current playback queue.

## Relationships

### Inherits From

- InvocationResponse

