

- GameKit
- GKMatchmaker
-  finishMatchmaking(for:) 

Instance Method

# finishMatchmaking(for:)

Informs the server when programmatic matchmaking finishes.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
func finishMatchmaking(for match: GKMatch)
```

## Parameters 

`match`  

The match that you are ready to start.

## Mentioned in 

Finding multiple players for a game

## Discussion

If you need to call the addPlayers(to:matchRequest:completionHandler:) method to fill the slots in an existing match, call the finishMatchmaking(for:) method when you have enough players and before you begin the match.

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

func cancel()

Cancels a matchmaking request.

func cancelPendingInvite(to: GKPlayer)

Cancels a pending invitation to another player.

