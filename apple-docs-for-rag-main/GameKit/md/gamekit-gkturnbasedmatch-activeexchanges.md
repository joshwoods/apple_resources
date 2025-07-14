

- GameKit
- GKTurnBasedMatch
-  activeExchanges 

Instance Property

# activeExchanges

The exchanges that the local player needs to accept or reject.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
var activeExchanges: [GKTurnBasedExchange]? { get }
```

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

var completedExchanges: [GKTurnBasedExchange]?

The exchange requests that all recipients replied to and the current participant needs to save.

var exchanges: [GKTurnBasedExchange]?

The exchange requests that are active or complete.

func saveMergedMatch(Data, withResolvedExchanges: [GKTurnBasedExchange], completionHandler: (((any Error)?) -> Void)?)

Saves match data for completed exchanges without ending the turn.

