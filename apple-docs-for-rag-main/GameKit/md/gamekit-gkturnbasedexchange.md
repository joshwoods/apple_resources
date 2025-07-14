

- GameKit
-  GKTurnBasedExchange 

Class

# GKTurnBasedExchange

Exchange request information that participants send in a turn-based match.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
class GKTurnBasedExchange
```

## Mentioned in 

Exchanging data between players in turn-based games

Sending messages to players in turn-based games

## Overview

GameKit sends exchange objects to GKTurnBasedEventListener protocol methods when the local player receives an exchange request or recipients reply to an exchange request. The exchange object encapsulates your custom game data that you want to communicate to other players.

You initiate an exchange request using the `GKTurnBasedMatch` sendExchange(to:data:localizableMessageKey:arguments:timeout:completionHandler:) method. Then GameKit sends the request to the recipients passing the exchange object to the `GKTurnBasedEventListener` player(_:receivedExchangeRequest:for:) protocol method. GameKit sets the status of the exchange object to GKTurnBasedExchangeStatus.active.

After all recipients respond to the request, using the reply(withLocalizableMessageKey:arguments:data:completionHandler:) method, or exceed the time out specified in the request, GameKit sends the exchange to the sender and the current participant. GameKit sets the exchange status to GKTurnBasedExchangeStatus.complete and then passes it to the `GKTurnBasedEventListener` player(_:receivedExchangeReplies:forCompletedExchange:for:) method.

Before the current participant ends their turn, save the completed exchanges using the `GKTurnBasedMatch` saveMergedMatch(_:withResolvedExchanges:completionHandler:) method. Get the exchanges from the match object using the completedExchanges property. Alternatively, save exchange data in the player(_:receivedExchangeReplies:forCompletedExchange:for:) protocol method when all recipients reply to specific exchange requests.

To cancel an active or complete exchange, use the cancel(withLocalizableMessageKey:arguments:completionHandler:) method. GameKit notifies the recipients when the player cancels an exchange, using the `GKTurnBasedEventListener` player(_:receivedExchangeCancellation:for:) protocol method.

## Topics

### Retrieving Exchange Details

var exchangeID: String

The identifier for the exchange request.

var sender: GKTurnBasedParticipant

The participant who sends the exchange request to recipients.

var recipients: [GKTurnBasedParticipant]

The participants who receives the exchange request.

var data: Data?

The game-specific exchange data that GameKit sends to participants.

var message: String?

A localized message from the sender to the recipients of an exchange request.

var sendDate: Date

The date that the sender initiates the exchange request.

var timeoutDate: Date?

The date that the recipients must reply by before the exchange request times out.

### Replying to Exchange Requests

func reply(withLocalizableMessageKey: String, arguments: [String], data: Data, completionHandler: (((any Error)?) -> Void)?)

Replies to an exchange request on behalf of a recipient.

var replies: [GKTurnBasedExchangeReply]?

The replies from recipients of the exchange request.

var status: GKTurnBasedExchangeStatus

The status of the exchange request.

enum GKTurnBasedExchangeStatus

The status of an exchange or reply.

var completionDate: Date?

The date when all recipients of the exchange request reply.

### Canceling Exchange Requests

func cancel(withLocalizableMessageKey: String, arguments: [String], completionHandler: (((any Error)?) -> Void)?)

Cancels an exchange request.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Turn-based games

Creating turn-based games

Develop games where multiple players take turns and can exchange data while waiting for their turn.

Starting turn-based matches and passing turns between players

Let Game Center store and forward match data between players in a turn-based game.

Sending messages to players in turn-based games

Notify players of match events by sending messages and game data.

Exchanging data between players in turn-based games

Add the ability for players to exchange game data and send messages while waiting for their turns.

class GKTurnBasedMatchmakerViewController

An interface that allows a player to invite other players to a turn-based match and automatch to fill any empty slots.

class GKTurnBasedMatch

An object that encapsulates the match data for games where players take turns.

class GKTurnBasedParticipant

A participant in a turn-based match.

protocol GKTurnBasedEventListener

The protocol that handles turn-based and data-exchange events between participants in a match.

class GKTurnBasedExchangeReply

Details about a recipient’s response to an exchange request.

GKGameCenterBadgingDisabled

A Boolean value indicating whether GameKit can add badges to a turn-based game icon.

