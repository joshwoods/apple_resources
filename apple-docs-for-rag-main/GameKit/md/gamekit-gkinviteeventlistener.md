

- GameKit
-  GKInviteEventListener 

Protocol

# GKInviteEventListener

A protocol that handles invite events from Game Center.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
protocol GKInviteEventListener
```

## Mentioned in 

Finding multiple players for a game

## Overview

Implement the methods in the GKInviteEventListener protocol to accept invitations from other players or handle when other players accept invitations from the local player.

Adopt the GKLocalPlayerListener protocol to listen for and handle a variety of Game Center events for player accounts instead of the individual GKChallengeListener, GKInviteEventListener, GKSavedGameListener, and GKTurnBasedEventListener protocols.

For details, see Finding multiple players for a game.

## Topics

### Starting a New Match

func player(GKPlayer, didAccept: GKInvite)

Handles the event when the local player accepts an invitation from another player.

func player(GKPlayer, didRequestMatchWithRecipients: [GKPlayer])

Handles the event when the local player sends other players an invitation to join a match.

func player(GKPlayer, didRequestMatchWithPlayers: [String])

Handles the event when the local player sends other players an invitation to join a match.

Deprecated

## Relationships

### Inherited By

- GKLocalPlayerListener

## See Also

### Real-time games

Creating real-time games

Develop games where multiple players interact in real time.

Finding multiple players for a game

Discover and invite other players to participate in a real-time game.

Exchanging data between players in real-time games

Send data between players in a real-time multiplayer game.

Adding voice chat to multiplayer games

Enable players to voice chat with all, or groups of, players in a multiplayer game.

Matchmaking rules

Game Center applies different type of rules you create in a particular order to find the best matches.

class GKMatchRequest

An object that encapsulates the parameters to create a real-time or turn-based match.

class GKMatchmaker

An object that creates matches with other players without presenting an interface to the players.

class GKMatchmakerViewController

An interface that allows a player to invite other players to a real-time game and automatch to fill any empty slots.

class GKInvite

An invitation to join a match sent to the local player from another player.

class GKMatch

A peer-to-peer network between a group of players that sign into Game Center.

