

- GameKit
- GKTurnBasedExchangeReply
-  recipient 

Instance Property

# recipient

The participant who replies to the exchange request.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
var recipient: GKTurnBasedParticipant { get }
```

## See Also

### Retrieving Reply Details

var data: Data?

The game-specific data that the recipent provides in the exchange request reply.

var message: String?

A message from the recipient to the sender of the exchange request.

var replyDate: Date

The date the recipient replies to the exchange request.

