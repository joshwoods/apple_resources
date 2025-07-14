

- SiriKit Cloud Media
-  PlayMediaIntentHandlingResolvePlayShuffledInvocationResponse 

Object

# PlayMediaIntentHandlingResolvePlayShuffledInvocationResponse

Your service’s response to a request to resolve whether a play media intent requests a shuffled queue.

SiriKit Cloud Media 1.0.2+

``` source
object PlayMediaIntentHandlingResolvePlayShuffledInvocationResponse
```

## Properties

`result`

PlayMediaIntentHandlingResolvePlayShuffledInvocationResponse.Result

 (Required) 

The result of processing the intent.

`method`

`string`

 (Required) 

The action your service takes to process this intent.

Value: `PlayMediaIntentHandling.resolvePlayShuffled`

## Topics

### Specifying a Result

object PlayMediaIntentHandlingResolvePlayShuffledInvocationResponse.Result

The result of resolving whether a play media intent shuffles the playback queue.

## Relationships

### Inherits From

- InvocationResponse

