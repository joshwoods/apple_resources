

- SiriKit Cloud Media
-  Constraints 

Object

# Constraints

Client-originated limitations on how to process a request, such as including explicit content and how much content the client device can receive in a response.

SiriKit Cloud Media 1.0.2+

``` source
object Constraints
```

## Properties

`allowExplicitContent`

`boolean`

An indicator of whether it’s OK for your service to provide explicit content.

Default: `true`

`maximumQueueSegmentItemCount`

`uint32`

The maximum number of pieces to provide in a Queue.

Default: `1000`

Minimum: `50`

Maximum: `1000`

`updateUserTasteProfile`

`boolean`

An indicator of whether to use these interactions to update your service’s model of the user’s likes and dislikes.

Default: `true`

## See Also

### Requests

object Invocation

Properties that clients include in requests to all intent endpoints.

object Session

Information the client provides about a sequence of requests and responses to process an intent.

object PlayerContext

Information about the current playback content.

object InvocationResponse

Properties to include in responses from all intent endpoints.

