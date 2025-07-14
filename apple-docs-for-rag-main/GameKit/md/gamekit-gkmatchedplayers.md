

- GameKit
-  GKMatchedPlayers 

Class

# GKMatchedPlayers

An object that represents matchmaking results, including the players that join the match and their properties that matchmaking rules uses.

iOS 17.2+iPadOS 17.2+Mac Catalyst 17.2+macOS 14.2+tvOS 17.2+visionOS 1.1+

``` source
class GKMatchedPlayers
```

## Overview

If the properties and `playersProperties` properties are `nil`, Game Center didn’t use matchmaking rules to find the players. For more information, see Matchmaking rules.

## Topics

### Getting players

var players: [GKPlayer]

The players that join the match.

### Matchmaking using rules

var properties: [String : Any]?

The local player’s properties that matchmaking rules uses to find the players, with some additions.

var playerProperties: [GKPlayer : [String : Any]]?

The properties for other players that matchmaking rules uses to find players, with some additions.

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

### Matching players

func findMatch(for: GKMatchRequest, withCompletionHandler: ((GKMatch?, (any Error)?) -> Void)?)

Initiates a request to find players for a peer-to-peer match.

func findPlayers(forHostedRequest: GKMatchRequest, withCompletionHandler: (([GKPlayer]?, (any Error)?) -> Void)?)

Initiates a request to find players for a hosted match.

func findMatchedPlayers(GKMatchRequest, withCompletionHandler: (GKMatchedPlayers?, (any Error)?) -> Void)

Initiates a request to find players for a hosted match that uses matchmaking rules.

func addPlayers(to: GKMatch, matchRequest: GKMatchRequest, completionHandler: (((any Error)?) -> Void)?)

Invites additional players to an existing match.

func finishMatchmaking(for: GKMatch)

Informs the server when programmatic matchmaking finishes.

func cancel()

Cancels a matchmaking request.

func cancelPendingInvite(to: GKPlayer)

Cancels a pending invitation to another player.

