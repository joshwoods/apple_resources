

- GameKit
- GKTurnBasedEventListener
-  player(\_:receivedExchangeReplies:forCompletedExchange:for:) 

Instance Method

# player(\_:receivedExchangeReplies:forCompletedExchange:for:)

Handles when all recipients of an exchange request respond.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
optional func player(
    _ player: GKPlayer,
    receivedExchangeReplies replies: [GKTurnBasedExchangeReply],
    forCompletedExchange exchange: GKTurnBasedExchange,
    for match: GKTurnBasedMatch
)
```

## Parameters 

`player`  

The player who receives this turn-based event.

`replies`  

The replies from other participants to the exchange request.

`exchange`  

The exchange request that the recipients reply to.

`match`  

The match related to this turn-based event.

## Mentioned in 

Exchanging data between players in turn-based games

## Discussion

GameKit sends this turn-based event to the current participant and the participant who initiates the exchange request.

If your game isn’t running or is in the background on participant devices, a notification containing the localized message you provide appears. When the participant taps or clicks the notification, GameKit launches or brings the game to the foreground and then invokes the player(_:receivedExchangeReplies:forCompletedExchange:for:) method.

## See Also

### Handling Data Exchanges

func player(GKPlayer, receivedExchangeRequest: GKTurnBasedExchange, for: GKTurnBasedMatch)

Handles when the local player receives an exchange request from another participant.

func player(GKPlayer, receivedExchangeCancellation: GKTurnBasedExchange, for: GKTurnBasedMatch)

Handles when the sender cancels an exchange request they intiated.

