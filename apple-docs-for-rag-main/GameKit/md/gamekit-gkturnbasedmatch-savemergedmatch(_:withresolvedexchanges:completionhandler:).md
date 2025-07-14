

- GameKit
- GKTurnBasedMatch
-  saveMergedMatch(\_:withResolvedExchanges:completionHandler:) 

Instance Method

# saveMergedMatch(\_:withResolvedExchanges:completionHandler:)

Saves match data for completed exchanges without ending the turn.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
func saveMergedMatch(
    _ matchData: Data,
    withResolvedExchanges exchanges: [GKTurnBasedExchange],
    completionHandler: (((any Error)?) -> Void)? = nil
)
```

``` source
func saveMergedMatch(
    _ matchData: Data,
    withResolvedExchanges exchanges: [GKTurnBasedExchange]
) async throws
```

## Parameters 

`matchData`  

Your game-specific data representing the match state including the resolved exchange data.

`exchanges`  

The completed exchanges that you resolve or merge into the match data.

`completionHandler`  

The block that GameKit calls when it completes the request.

The block receives the following parameter:

*error*  
Describes an error if it occurs, or `nil` if the operation completes.

## Mentioned in 

Exchanging data between players in turn-based games

## Discussion

Use this method to save the exchange data in the match’s completedExchanges property before the current participant ends their turn, forfeits a match, or ends a match. Alternatively, invoke this method from the player(_:receivedExchangeReplies:forCompletedExchange:for:) protocol method as recipients reply to individual exchange requests.

This method removes the exchanges from the current participant’s `completedExchanges` property and all participant’s exchanges property. So retain your game-specific exchange data and merge it into the match data, before you invoke this method.

## See Also

### Exchanging Data Between Participants

func sendExchange(to: [GKTurnBasedParticipant], data: Data, localizableMessageKey: String, arguments: [String], timeout: TimeInterval, completionHandler: ((GKTurnBasedExchange?, (any Error)?) -> Void)?)

Sends an exchange request that contains your game data to one or more participants.

Exchange Timeouts

The amount of time that passes before an exchange times out.

var exchangeDataMaximumSize: Int

The maximum size of the exchange data.

var exchangeMaxInitiatedExchangesPerPlayer: Int

The maximum number of exchanges the local player can initiate.

var activeExchanges: [GKTurnBasedExchange]?

The exchanges that the local player needs to accept or reject.

var completedExchanges: [GKTurnBasedExchange]?

The exchange requests that all recipients replied to and the current participant needs to save.

var exchanges: [GKTurnBasedExchange]?

The exchange requests that are active or complete.

