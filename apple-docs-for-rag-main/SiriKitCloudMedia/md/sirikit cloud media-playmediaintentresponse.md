

- SiriKit Cloud Media
-  PlayMediaIntentResponse 

Object

# PlayMediaIntentResponse

A structure that contains a response code indicating how your service handles a play media intent.

SiriKit Cloud Media 1.0.2+

``` source
object PlayMediaIntentResponse
```

## Properties

`class`

`string`

 (Required) 

The specific type of response.

Value: `PlayMediaIntentResponse`

`code`

PlayMediaIntentResponseCode

 (Required) 

A response code that indicates whether your service can play the media item.

## Relationships

### Inherits From

- IntentResponse

## See Also

### Handling a Play Media Intent

object PlayMediaIntentHandlingHandleInvocationResponse

Your service’s response to a request to handle a fully resolved play media intent.

type PlayMediaIntentResponseCode

Codes your service can return when handling a play media intent.

