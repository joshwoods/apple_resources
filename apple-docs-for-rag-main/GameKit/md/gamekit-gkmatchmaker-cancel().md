

- GameKit
- GKMatchmaker
-  cancel() 

Instance Method

# cancel()

Cancels a matchmaking request.

iOS 4.1+iPadOS 4.1+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+

``` source
func cancel()
```

## Discussion

GameKit sends a GKError.Code.cancelled error to the completion handler of either the findMatch(for:withCompletionHandler:) or findPlayers(forHostedRequest:withCompletionHandler:) method.

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

func cancelPendingInvite(to: GKPlayer)

Cancels a pending invitation to another player.

