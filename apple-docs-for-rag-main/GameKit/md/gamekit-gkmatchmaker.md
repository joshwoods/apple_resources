

- GameKit
-  GKMatchmaker 

Class

# GKMatchmaker

An object that creates matches with other players without presenting an interface to the players.

iOS 4.1+iPadOS 4.1+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+

``` source
class GKMatchmaker
```

## Mentioned in 

Finding players with similar skill levels

Finding multiple players for a game

## Overview

Use the `GKMatchmaker` class to auto-match players for a quicker game start, programmatically invite specific players, or implement your own interface for players to invite other players. If you want to present a familiar matchmaking GameKit interface to players, instead use either the GKMatchmakerViewController or GKTurnBasedMatchmakerViewController class.

If you host a game on your own server, you can also use this class to find Game Center players. That is, you implement the networking and communication between the players through your own servers not Game Center.

To find players using this class, create a GKMatchRequest object and configure it according to the parameters of your game. Then, pass the match request and a handler using the findMatch(for:withCompletionHandler:) method, or the findPlayers(forHostedMatchRequest:withCompletionHandler:) method for hosted games, to the shared `GKMatchmaker` object.

GameKit calls the handler when players accept their invitations. Implement the handler to set the delegate of the GKMatch object that GameKit sends and start the game when there are enough players.

If the match doesn’t have enough players (for example, some players decline their invitations), you can create another match request and call the addPlayers(to:matchRequest:completionHandler:) method repeatedly until the match’s expectedPlayerCount property is zero. When you have enough players to start the match, call the finishMatchmaking(for:) method to end the matchmaking process.

If you provide a SharePlay interface for inviting players, use the startGroupActivity(playerHandler:) and stopGroupActivity() methods to create a group activity on behalf of the player.

## Topics

### Retrieving the shared matchmaker

class func shared() -> GKMatchmaker

Returns the singleton matchmaker instance.

### Receiving invitations from other players

func match(for: GKInvite, completionHandler: ((GKMatch?, (any Error)?) -> Void)?)

Creates a match from an invitation that the local player accepts.

### Matching players

func findMatch(for: GKMatchRequest, withCompletionHandler: ((GKMatch?, (any Error)?) -> Void)?)

Initiates a request to find players for a peer-to-peer match.

func findPlayers(forHostedRequest: GKMatchRequest, withCompletionHandler: (([GKPlayer]?, (any Error)?) -> Void)?)

Initiates a request to find players for a hosted match.

func findMatchedPlayers(GKMatchRequest, withCompletionHandler: (GKMatchedPlayers?, (any Error)?) -> Void)

Initiates a request to find players for a hosted match that uses matchmaking rules.

class GKMatchedPlayers

An object that represents matchmaking results, including the players that join the match and their properties that matchmaking rules uses.

func addPlayers(to: GKMatch, matchRequest: GKMatchRequest, completionHandler: (((any Error)?) -> Void)?)

Invites additional players to an existing match.

func finishMatchmaking(for: GKMatch)

Informs the server when programmatic matchmaking finishes.

func cancel()

Cancels a matchmaking request.

func cancelPendingInvite(to: GKPlayer)

Cancels a pending invitation to another player.

### Finding players who request matches

func queryActivity(completionHandler: ((Int, (any Error)?) -> Void)?)

Finds the number of players, across player groups, who recently requested a match.

func queryPlayerGroupActivity(Int, withCompletionHandler: ((Int, (any Error)?) -> Void)?)

Finds the number of players in a player group who recently requested a match.

func queryQueueActivity(String, withCompletionHandler: ((Int, (any Error)?) -> Void)?)

Finds the number of players in a specific queue who recently requested a match.

### Looking for nearby players

func startBrowsingForNearbyPlayers(handler: ((GKPlayer, Bool) -> Void)?)

Finds nearby players through Bluetooth or WiFi on the same subnet.

func stopBrowsingForNearbyPlayers()

Stops finding nearby players.

### Starting matches using SharePlay

func startGroupActivity(playerHandler: (GKPlayer) -> Void)

Begins a SharePlay activity for your game when a FaceTime call is active.

func stopGroupActivity()

Ends a SharePlay activity for the entire group, which the local player activates.

### Deprecated

Deprecated Symbols

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

class GKMatchmakerViewController

An interface that allows a player to invite other players to a real-time game and automatch to fill any empty slots.

protocol GKInviteEventListener

A protocol that handles invite events from Game Center.

class GKInvite

An invitation to join a match sent to the local player from another player.

class GKMatch

A peer-to-peer network between a group of players that sign into Game Center.

