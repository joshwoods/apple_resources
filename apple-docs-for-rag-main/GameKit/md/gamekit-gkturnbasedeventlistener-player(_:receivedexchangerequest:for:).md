

- GameKit
- GKTurnBasedEventListener
-  player(\_:receivedExchangeRequest:for:) 

Instance Method

# player(\_:receivedExchangeRequest:for:)

Handles when the local player receives an exchange request from another participant.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
optional func player(
    _ player: GKPlayer,
    receivedExchangeRequest exchange: GKTurnBasedExchange,
    for match: GKTurnBasedMatch
)
```

## Parameters 

`player`  

The player who receives this turn-based event.

`exchange`  

The exchange request sent from the other participant.

`match`  

The match related to this turn-based event.

## Mentioned in 

Exchanging data between players in turn-based games

## Discussion

Reply to this exchange request using the `GKTurnBasedExchange` reply(withLocalizableMessageKey:arguments:data:completionHandler:) method.

## See Also

### Handling Data Exchanges

func player(GKPlayer, receivedExchangeReplies: [GKTurnBasedExchangeReply], forCompletedExchange: GKTurnBasedExchange, for: GKTurnBasedMatch)

Handles when all recipients of an exchange request respond.

func player(GKPlayer, receivedExchangeCancellation: GKTurnBasedExchange, for: GKTurnBasedMatch)

Handles when the sender cancels an exchange request they intiated.

