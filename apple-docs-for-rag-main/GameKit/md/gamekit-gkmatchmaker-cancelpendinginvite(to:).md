

- GameKit
- GKMatchmaker
-  cancelPendingInvite(to:) 

Instance Method

# cancelPendingInvite(to:)

Cancels a pending invitation to another player.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
func cancelPendingInvite(to player: GKPlayer)
```

## Parameters 

`player`  

The player that GameKit sends the invitation to.

## See Also

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

