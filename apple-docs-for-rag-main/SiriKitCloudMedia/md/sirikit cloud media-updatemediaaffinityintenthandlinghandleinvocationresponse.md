

- SiriKit Cloud Media
-  UpdateMediaAffinityIntentHandlingHandleInvocationResponse 

Object

# UpdateMediaAffinityIntentHandlingHandleInvocationResponse

Your service’s response to a request to handle a fully resolved update media affinity intent.

SiriKit Cloud Media 1.0.2+

``` source
object UpdateMediaAffinityIntentHandlingHandleInvocationResponse
```

## Properties

`result`

UpdateMediaAffinityIntentHandlingHandleInvocationResponse.Result

 (Required) 

The results of processing the intent.

`method`

`string`

 (Required) 

The action your service takes to process this intent.

Value: `UpdateMediaAffinityIntentHandling.handle`

## Topics

### Specifying the Result

object UpdateMediaAffinityIntentHandlingHandleInvocationResponse.Result

The result of handling an intent to update media affinity.

## Relationships

### Inherits From

- InvocationResponse

## See Also

### Handling an Update Media Affinity Intent

object UpdateMediaAffinityIntentResponse

A structure that contains a response code indicating how your service handles an update media affinity intent.

type UpdateMediaAffinityIntentResponseCode

Codes your service can return when handling an update media affinity intent.

