

- SiriKit Cloud Media
-  Invocation 

Object

# Invocation

Properties that clients include in requests to all intent endpoints.

SiriKit Cloud Media 1.0.2+

``` source
object Invocation
```

## Properties

`method`

`string`

 (Required) 

The action your service takes to process this intent.

`params`

Invocation.Params

 (Required) 

Additional properties specific to an invocation.

`session`

Session

The client’s information about this series of requests and responses.

## Topics

### Accessing the Details of a Request

object Invocation.Params

The parameters of a client’s request.

## Relationships

### Inherited By

- AddMediaIntentHandlingInvocation
- PlayMediaIntentHandlingInvocation
- UpdateMediaAffinityIntentHandlingInvocation

## See Also

### Requests

object Session

Information the client provides about a sequence of requests and responses to process an intent.

object Constraints

Client-originated limitations on how to process a request, such as including explicit content and how much content the client device can receive in a response.

object PlayerContext

Information about the current playback content.

object InvocationResponse

Properties to include in responses from all intent endpoints.

