

- GameKit
-  GKInvite 

Class

# GKInvite

An invitation to join a match sent to the local player from another player.

iOS 4.1+iPadOS 4.1+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+

``` source
class GKInvite
```

## Overview

Your game never directly creates `GKInvite` objects. Instead, these objects are created by GameKit and delivered to your game’s matchmaking event handler. The properties of the invitation object describe the match to which another player invites the local player.

## Topics

### Getting Properties

var sender: GKPlayer

The player who sends the invitation.

var playerAttributes: UInt32

The player attributes for the match.

var playerGroup: Int

The player group for the match.

var isHosted: Bool

A Boolean value that indicates whether you host the game on your own servers.

var inviter: String

The identifier for the player who sends the invitation.

Deprecated

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

protocol GKInviteEventListener

A protocol that handles invite events from Game Center.

class GKMatch

A peer-to-peer network between a group of players that sign into Game Center.

