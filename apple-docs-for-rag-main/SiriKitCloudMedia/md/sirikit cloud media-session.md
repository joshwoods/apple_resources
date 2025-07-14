

- SiriKit Cloud Media
-  Session 

Object

# Session

Information the client provides about a sequence of requests and responses to process an intent.

SiriKit Cloud Media 1.0.2+

``` source
object Session
```

## Properties

`identifier`

`string`

 (Required) 

A stable identifier for all requests and responses relating to a specific intent.

Minimum length: `1`

Maximum length: `128`

`constraints`

Constraints

 (Required) 

Client limitations on content quantity and type that apply to all responses your service makes for this session.

`requested`

`date-time`

 (Required) 

The time the user initiates the request.

`deadline`

`date-time`

 (Required) 

The time by which the client expects a response from your service to provide a real-time interaction with the user.

`playerContext`

PlayerContext

Information about content the client is playing, if any.

`version`

`string`

 (Required) 

The version of the `SiriKitMediaAPI` library the client is using.

Value: `/[0-9]+\.[0-9]+\.[0-9]+/`

## See Also

### Requests

object Invocation

Properties that clients include in requests to all intent endpoints.

object Constraints

Client-originated limitations on how to process a request, such as including explicit content and how much content the client device can receive in a response.

object PlayerContext

Information about the current playback content.

object InvocationResponse

Properties to include in responses from all intent endpoints.

