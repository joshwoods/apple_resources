

- SiriKit Cloud Media
-  InvocationResponse 

Object

# InvocationResponse

Properties to include in responses from all intent endpoints.

SiriKit Cloud Media 1.0.2+

``` source
object InvocationResponse
```

## Properties

`result`

InvocationResponse.Result

 (Required) 

The outcome of handling the intent.

`method`

`string`

 (Required) 

The action your service takes to process this intent.

`metrics`

ExecutionMetrics

Performance details about processing the request.

`debug`

ServiceDebugReference

A URI for additional data about this request. Only include this property in debugging or staging environments, not in production.

Maximum length: `2000`

## Topics

### Providing a Result

object InvocationResponse.Result

The outcome of handling an intent.

### Instrumenting Your Service

object ExecutionMetrics

Timing information to isolate service performance from network delays.

type ServiceDebugReference

A URI that references debugging information for a request.

## Relationships

### Inherited By

- AddMediaIntentHandlingConfirmInvocationResponse
- AddMediaIntentHandlingHandleInvocationResponse
- AddMediaIntentHandlingResolveMediaDestinationInvocationResponse
- AddMediaIntentHandlingResolveMediaItemsInvocationResponse
- PlayMediaIntentHandlingHandleInvocationResponse
- PlayMediaIntentHandlingResolveMediaItemsInvocationResponse
- PlayMediaIntentHandlingResolvePlayShuffledInvocationResponse
- PlayMediaIntentHandlingResolvePlaybackQueueLocationInvocationResponse
- PlayMediaIntentHandlingResolvePlaybackRepeatModeInvocationResponse
- PlayMediaIntentHandlingResolveResumePlaybackInvocationResponse
- ProtocolExceptionInvocationResponse
- UpdateMediaAffinityIntentHandlingHandleInvocationResponse
- UpdateMediaAffinityIntentHandlingResolveAffinityTypeInvocationResponse
- UpdateMediaAffinityIntentHandlingResolveMediaItemsInvocationResponse

## See Also

### Requests

object Invocation

Properties that clients include in requests to all intent endpoints.

object Session

Information the client provides about a sequence of requests and responses to process an intent.

object Constraints

Client-originated limitations on how to process a request, such as including explicit content and how much content the client device can receive in a response.

object PlayerContext

Information about the current playback content.

