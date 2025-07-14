

- GameKit
- GKTurnBasedExchange
-  completionDate 

Instance Property

# completionDate

The date when all recipients of the exchange request reply.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
var completionDate: Date? { get }
```

## Discussion

The date the exchange status property becomes GKTurnBasedExchangeStatus.complete.

## See Also

### Replying to Exchange Requests

func reply(withLocalizableMessageKey: String, arguments: [String], data: Data, completionHandler: (((any Error)?) -> Void)?)

Replies to an exchange request on behalf of a recipient.

var replies: [GKTurnBasedExchangeReply]?

The replies from recipients of the exchange request.

var status: GKTurnBasedExchangeStatus

The status of the exchange request.

enum GKTurnBasedExchangeStatus

The status of an exchange or reply.

