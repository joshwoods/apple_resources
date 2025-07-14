

- GameKit
- GKTurnBasedEventListener
-  player(\_:receivedExchangeCancellation:for:) 

Instance Method

# player(\_:receivedExchangeCancellation:for:)

Handles when the sender cancels an exchange request they intiated.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
optional func player(
    _ player: GKPlayer,
    receivedExchangeCancellation exchange: GKTurnBasedExchange,
    for match: GKTurnBasedMatch
)
```

## Parameters 

`player`  

The player who receives this turn-based event.

`exchange`  

The exchange request that the sender cancels.

`match`  

The match related to this turn-based event.

## Mentioned in 

Exchanging data between players in turn-based games

## See Also

### Handling Data Exchanges

func player(GKPlayer, receivedExchangeRequest: GKTurnBasedExchange, for: GKTurnBasedMatch)

Handles when the local player receives an exchange request from another participant.

func player(GKPlayer, receivedExchangeReplies: [GKTurnBasedExchangeReply], forCompletedExchange: GKTurnBasedExchange, for: GKTurnBasedMatch)

Handles when all recipients of an exchange request respond.

