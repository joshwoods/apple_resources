

- SiriKit Cloud Media
-  PlayMediaIntentHandlingHandleInvocationResponse 

Object

# PlayMediaIntentHandlingHandleInvocationResponse

Your service’s response to a request to handle a fully resolved play media intent.

SiriKit Cloud Media 1.0.2+

``` source
object PlayMediaIntentHandlingHandleInvocationResponse
```

## Properties

`result`

PlayMediaIntentHandlingHandleInvocationResponse.Result

 (Required) 

The results of processing the intent.

`method`

`string`

 (Required) 

The action your service takes to process this intent.

Value: `PlayMediaIntentHandling.handle`

## Topics

### Specifying a Result

object PlayMediaIntentHandlingHandleInvocationResponse.Result

The result of handling an intent to play a media item.

## Relationships

### Inherits From

- InvocationResponse

## See Also

### Handling a Play Media Intent

object PlayMediaIntentResponse

A structure that contains a response code indicating how your service handles a play media intent.

type PlayMediaIntentResponseCode

Codes your service can return when handling a play media intent.

