

- GameKit
- GKTurnBasedExchangeReply
-  message 

Instance Property

# message

A message from the recipient to the sender of the exchange request.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
var message: String? { get }
```

## See Also

### Retrieving Reply Details

var data: Data?

The game-specific data that the recipent provides in the exchange request reply.

var recipient: GKTurnBasedParticipant

The participant who replies to the exchange request.

var replyDate: Date

The date the recipient replies to the exchange request.

