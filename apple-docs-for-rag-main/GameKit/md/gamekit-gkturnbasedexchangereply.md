

- GameKit
-  GKTurnBasedExchangeReply 

Class

# GKTurnBasedExchangeReply

Details about a recipient’s response to an exchange request.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
class GKTurnBasedExchangeReply
```

## Mentioned in 

Exchanging data between players in turn-based games

## Overview

When you accept an exchange request using the reply(withLocalizableMessageKey:arguments:data:completionHandler:) method, GameKit sends a `GKTurnBasedExchangeReply` object to participants using the player(_:receivedExchangeReplies:forCompletedExchange:for:) protocol method. You can also get responses to exchange requests from the GKTurnBasedExchange object using the replies parameter.

## Topics

### Retrieving Reply Details

var data: Data?

The game-specific data that the recipent provides in the exchange request reply.

var message: String?

A message from the recipient to the sender of the exchange request.

var recipient: GKTurnBasedParticipant

The participant who replies to the exchange request.

var replyDate: Date

The date the recipient replies to the exchange request.

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

class GKTurnBasedExchange

Exchange request information that participants send in a turn-based match.

GKGameCenterBadgingDisabled

A Boolean value indicating whether GameKit can add badges to a turn-based game icon.

