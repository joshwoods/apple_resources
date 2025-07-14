

- SiriKit Cloud Media
-  UpdateMediaAffinityIntentResponse 

Object

# UpdateMediaAffinityIntentResponse

A structure that contains a response code indicating how your service handles an update media affinity intent.

SiriKit Cloud Media 1.0.2+

``` source
object UpdateMediaAffinityIntentResponse
```

## Properties

`class`

`string`

 (Required) 

The specific type of response.

Value: `UpdateMediaAffinityIntentResponse`

`code`

UpdateMediaAffinityIntentResponseCode

 (Required) 

A response code that indicates whether your service can play the media item.

## Relationships

### Inherits From

- IntentResponse

## See Also

### Handling an Update Media Affinity Intent

object UpdateMediaAffinityIntentHandlingHandleInvocationResponse

Your service’s response to a request to handle a fully resolved update media affinity intent.

type UpdateMediaAffinityIntentResponseCode

Codes your service can return when handling an update media affinity intent.

