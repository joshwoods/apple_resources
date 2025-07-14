

- GameKit
-  GKMatch 

Class

# GKMatch

A peer-to-peer network between a group of players that sign into Game Center.

iOS 4.1+iPadOS 4.1+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+

``` source
class GKMatch
```

## Mentioned in 

Finding multiple players for a game

Assigning players to teams using rules

## Overview

Matches provide a mechanism for a player to send both game and voice data to other players.

You never create a `GKMatch` object directly. Instead, GameKit passes a match object to a GKMatchmakerViewControllerDelegate method or a GKMatchmaker handler when you set up a multiplayer game. For details, see Finding multiple players for a game.

If you use the GKMatchmakerViewController class to find players, implement the matchmakerViewController(_:didFind:) delegate method to set the match delegate. If you use the GKMatchmaker class, set the match delegate in the handler you pass to the findMatch(for:withCompletionHandler:) method.

You can begin exchanging data when two or more players join the match. Implement the match(_:player:didChange:) delegate method to track when players connect or disconnect from the match. Then use either the sendData(toAllPlayers:with:) or the send(_:to:dataMode:) method to send data. To process the data on the recipient side, implement the match(_:didReceive:fromRemotePlayer:) delegate method.

To implement voice chat, use the voiceChat(withName:) method to create one or more voice channels represented by the returned GKVoiceChat object.

When you’re finished with a match, call the disconnect() method and set the match’s delegate to `nil`. Otherwise, GameKit may send match(_:player:didChange:) to the delegate until all players disconnect from the match.

## Topics

### Setting the delegate

var delegate: (any GKMatchDelegate)?

The delegate that handles communication between players in a match.

protocol GKMatchDelegate

An object that receives connection status and data transmitted in a multiplayer game.

### Working with other players

var expectedPlayerCount: Int

The remaining number of players invited but not yet connected to the match.

var players: [GKPlayer]

The players that join the match.

### Sending data to other players

func chooseBestHostingPlayer(completionHandler: (GKPlayer?) -> Void)

Determines the best player in the game to act as the server for a client-server topology.

func send(Data, to: [GKPlayer], dataMode: GKMatch.SendDataMode) throws

Transmits data to one or more players connected to the match.

func sendData(toAllPlayers: Data, with: GKMatch.SendDataMode) throws

Transmits data to all players connected to the match.

enum SendDataMode

The mechanism used to transmit data to other players.

### Joining a voice chat

func voiceChat(withName: String) -> GKVoiceChat?

Joins the local player to a voice channel.

Deprecated

### Getting matchmaking properties

var properties: [String : Any]?

The local player’s properties that matchmaking rules used to find the players with some additions.

var playerProperties: [GKPlayer : [String : Any]]?

The properties for other players that matchmaking rules uses to find players, with some additions.

### Finishing the match

func disconnect()

Disconnects the local player from the match.

func rematch(completionHandler: ((GKMatch?, (any Error)?) -> Void)?)

Creates a new match with the players from an existing match.

### Deprecated Methods and Properties

func chooseBestHostPlayer(completionHandler: (String?) -> Void)

Determines the best player in the game to act as the server for a client-server match.

Deprecated

var playerIDs: [String]?

The player identifiers for remote players in the match.

Deprecated

func send(Data, toPlayers: [String], with: GKMatch.SendDataMode) throws

Transmits data to a list of connected players.

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

class GKInvite

An invitation to join a match sent to the local player from another player.

