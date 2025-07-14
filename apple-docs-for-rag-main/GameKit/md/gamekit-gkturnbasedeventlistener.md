

- GameKit
-  GKTurnBasedEventListener 

Protocol

# GKTurnBasedEventListener

The protocol that handles turn-based and data-exchange events between participants in a match.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
protocol GKTurnBasedEventListener
```

## Mentioned in 

Starting turn-based matches and passing turns between players

Exchanging data between players in turn-based games

## Overview

To receive the `GKTurnBasedEventListener` call backs, register your game object with the local player object immediately after authentication.

```
GKLocalPlayer.local.register(self)
```

Adopt the GKLocalPlayerListener protocol to handle a variety of Game Center events instead of the individual GKChallengeListener, GKInviteEventListener, GKSavedGameListener, and GKTurnBasedEventListener protocols.

Then implement the player(_:receivedTurnEventFor:didBecomeActive:) and other `GKTurnBasedEventListener` protocol methods to handle turn-based events that occur throughout a match.

## Topics

### Handling Match-Related Events

func player(GKPlayer, receivedTurnEventFor: GKTurnBasedMatch, didBecomeActive: Bool)

Handles turn-based match events, such as accepting invitations, passing turns, and saving match data.

func player(GKPlayer, didRequestMatchWithOtherPlayers: [GKPlayer])

Handles when the player uses Game Center to start a match with other players.

func player(GKPlayer, matchEnded: GKTurnBasedMatch)

Handles when the match ends.

func player(GKPlayer, wantsToQuitMatch: GKTurnBasedMatch)

Handles when the current participant wants to quit a match.

func player(GKPlayer, didRequestMatchWithPlayers: [String])

Handles when the player uses Game Center to start a match with other players.

Deprecated

### Handling Data Exchanges

func player(GKPlayer, receivedExchangeRequest: GKTurnBasedExchange, for: GKTurnBasedMatch)

Handles when the local player receives an exchange request from another participant.

func player(GKPlayer, receivedExchangeReplies: [GKTurnBasedExchangeReply], forCompletedExchange: GKTurnBasedExchange, for: GKTurnBasedMatch)

Handles when all recipients of an exchange request respond.

func player(GKPlayer, receivedExchangeCancellation: GKTurnBasedExchange, for: GKTurnBasedMatch)

Handles when the sender cancels an exchange request they intiated.

## Relationships

### Inherited By

- GKLocalPlayerListener

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

class GKTurnBasedExchange

Exchange request information that participants send in a turn-based match.

class GKTurnBasedExchangeReply

Details about a recipient’s response to an exchange request.

GKGameCenterBadgingDisabled

A Boolean value indicating whether GameKit can add badges to a turn-based game icon.

