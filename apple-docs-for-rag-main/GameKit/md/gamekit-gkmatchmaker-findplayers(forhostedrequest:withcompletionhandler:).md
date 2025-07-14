

- GameKit
- GKMatchmaker
-  findPlayers(forHostedRequest:withCompletionHandler:) 

Instance Method

# findPlayers(forHostedRequest:withCompletionHandler:)

Initiates a request to find players for a hosted match.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
func findPlayers(
    forHostedRequest request: GKMatchRequest,
    withCompletionHandler completionHandler: (([GKPlayer]?, (any Error)?) -> Void)? = nil
)
```

``` source
func findPlayers(forHostedRequest request: GKMatchRequest) async throws -> [GKPlayer]
```

## Parameters 

`request`  

The configuration for the match.

`completionHandler`  

The block that GameKit calls when it completes the request.

This block receives the following parameters:

`players`  
The players that join the match. If unsuccessful, this parameter is `nil`.

`error`  
Describes an error if it occurs, or `nil` if the operation completes.

## Discussion

To find players using matchmaking rules, set the rules-related properties in `request` (queueName and optionally, properties) before you call this method. To get the properties of all players who join the match, use the findMatchedPlayers(_:withCompletionHandler:) method instead. For more information, see Matchmaking rules.

## See Also

### Matching players

func findMatch(for: GKMatchRequest, withCompletionHandler: ((GKMatch?, (any Error)?) -> Void)?)

Initiates a request to find players for a peer-to-peer match.

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

