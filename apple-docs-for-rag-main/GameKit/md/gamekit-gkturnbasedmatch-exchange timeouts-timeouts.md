

- GameKit
- GKTurnBasedMatch
-  Exchange Timeouts 

API Collection

# Exchange Timeouts

The amount of time that passes before an exchange times out.

## Topics

### Timeouts

var GKExchangeTimeoutDefault: TimeInterval

A one-day exchange request timeout.

var GKExchangeTimeoutNone: TimeInterval

An exchange request timeout that doesn’t expire.

## See Also

### Exchanging Data Between Participants

func sendExchange(to: [GKTurnBasedParticipant], data: Data, localizableMessageKey: String, arguments: [String], timeout: TimeInterval, completionHandler: ((GKTurnBasedExchange?, (any Error)?) -> Void)?)

Sends an exchange request that contains your game data to one or more participants.

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

func saveMergedMatch(Data, withResolvedExchanges: [GKTurnBasedExchange], completionHandler: (((any Error)?) -> Void)?)

Saves match data for completed exchanges without ending the turn.

