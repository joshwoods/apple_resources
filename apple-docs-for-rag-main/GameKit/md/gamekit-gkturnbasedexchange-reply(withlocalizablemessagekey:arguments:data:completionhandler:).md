

- GameKit
- GKTurnBasedExchange
-  reply(withLocalizableMessageKey:arguments:data:completionHandler:) 

Instance Method

# reply(withLocalizableMessageKey:arguments:data:completionHandler:)

Replies to an exchange request on behalf of a recipient.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
func reply(
    withLocalizableMessageKey key: String,
    arguments: [String],
    data: Data,
    completionHandler: (((any Error)?) -> Void)? = nil
)
```

``` source
func reply(
    withLocalizableMessageKey key: String,
    arguments: [String],
    data: Data
) async throws
```

## Parameters 

`key`  

The identifier for looking up the translated reply message in the default `Localized.strings` file. If you use a formatted string with specifiers, provide the arguments.

`arguments`  

A list of arguments to substitute into the localized string if it’s formatted and contains specifiers.

`data`  

The game-specific data associated with the reply.

`completionHandler`  

The block that GameKit calls when it completes the request.

The block receives the following parameter:

*error*  
Describes an error if it occurs, or `nil` if the operation completes.

## Mentioned in 

Exchanging data between players in turn-based games

## Discussion

To accept or decline an exchange request, invoke this method from the player(_:receivedExchangeRequest:for:) protocol method. Include game-specific details about the exchange in the `data` parameter. When all recipients reply or time out, GameKit invokes the player(_:receivedExchangeReplies:forCompletedExchange:for:) protocol method in the game instances of the sender and the current participant.

## See Also

### Replying to Exchange Requests

var replies: [GKTurnBasedExchangeReply]?

The replies from recipients of the exchange request.

var status: GKTurnBasedExchangeStatus

The status of the exchange request.

enum GKTurnBasedExchangeStatus

The status of an exchange or reply.

var completionDate: Date?

The date when all recipients of the exchange request reply.

