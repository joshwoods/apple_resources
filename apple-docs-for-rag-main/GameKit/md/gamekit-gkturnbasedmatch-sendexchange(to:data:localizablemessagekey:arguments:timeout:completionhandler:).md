

- GameKit
- GKTurnBasedMatch
-  sendExchange(to:data:localizableMessageKey:arguments:timeout:completionHandler:) 

Instance Method

# sendExchange(to:data:localizableMessageKey:arguments:timeout:completionHandler:)

Sends an exchange request that contains your game data to one or more participants.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
func sendExchange(
    to participants: [GKTurnBasedParticipant],
    data: Data,
    localizableMessageKey key: String,
    arguments: [String],
    timeout: TimeInterval,
    completionHandler: ((GKTurnBasedExchange?, (any Error)?) -> Void)? = nil
)
```

``` source
func sendExchange(
    to participants: [GKTurnBasedParticipant],
    data: Data,
    localizableMessageKey key: String,
    arguments: [String],
    timeout: TimeInterval
) async throws -> GKTurnBasedExchange
```

## Parameters 

`participants`  

The other participants, excluding the local player and inactive participants, that GameKit sends the exchange request to.

`data`  

The data that GameKit sends to the other participants.

`key`  

The identifier for looking up the translated message in the default `Localized.strings` file. If you use a formatted string with specifiers, provide the arguments.

`arguments`  

A list of arguments to substitute into the localized string if it’s formatted and contains specifiers.

`timeout`  

The length of time a participant has to respond to the exchange request. The maximum value is 90 days.

`completionHandler`  

The block that GameKit calls when it completes the request.

The block receives the following parameters:

exchange  
The exchange object that GameKit passes to the other participants.

*error*  
Describes an error if it occurs, or `nil` if the operation completes. An error occurs if any of the participants are inactive.

## Mentioned in 

Exchanging data between players in turn-based games

## Discussion

If your game isn’t running or is in the background on recipient devices, a notification containing the localized message you pass to this method appears. When the participant taps or clicks the notification, GameKit launches or brings the game to the foreground and then invokes the player(_:receivedExchangeRequest:for:) method.

Implement the player(_:receivedExchangeRequest:for:) protocol method to handle the exchange request — for example, show an interface on the receiver’s device to accept or reject the exchange.

## See Also

### Exchanging Data Between Participants

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

func saveMergedMatch(Data, withResolvedExchanges: [GKTurnBasedExchange], completionHandler: (((any Error)?) -> Void)?)

Saves match data for completed exchanges without ending the turn.

