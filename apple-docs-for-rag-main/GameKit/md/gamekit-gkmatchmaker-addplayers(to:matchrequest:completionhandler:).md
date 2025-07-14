

- GameKit
- GKMatchmaker
-  addPlayers(to:matchRequest:completionHandler:) 

Instance Method

# addPlayers(to:matchRequest:completionHandler:)

Invites additional players to an existing match.

iOS 4.1+iPadOS 4.1+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+

``` source
func addPlayers(
    to match: GKMatch,
    matchRequest: GKMatchRequest,
    completionHandler: (((any Error)?) -> Void)? = nil
)
```

``` source
func addPlayers(
    to match: GKMatch,
    matchRequest: GKMatchRequest
) async throws
```

## Parameters 

`match`  

The match to which GameKit adds the players.

`matchRequest`  

The configuration for the match.

`completionHandler`  

The block that GameKit calls when it completes the request.

This block receives the following parameters:

`error`  
Describes an error if it occurs, or `nil` if the operation completes.

## Discussion

Use this method to add more players to an existing match that doesn’t have enough players.

Important

Invoke this method for only one player connected to the match.

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

func finishMatchmaking(for: GKMatch)

Informs the server when programmatic matchmaking finishes.

func cancel()

Cancels a matchmaking request.

func cancelPendingInvite(to: GKPlayer)

Cancels a pending invitation to another player.

