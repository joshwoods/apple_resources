

- GameKit
- GKMatchmaker
-  findMatch(for:withCompletionHandler:) 

Instance Method

# findMatch(for:withCompletionHandler:)

Initiates a request to find players for a peer-to-peer match.

iOS 4.1+iPadOS 4.1+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+

``` source
func findMatch(
    for request: GKMatchRequest,
    withCompletionHandler completionHandler: ((GKMatch?, (any Error)?) -> Void)? = nil
)
```

``` source
func findMatch(for request: GKMatchRequest) async throws -> GKMatch
```

## Parameters 

`request`  

The configuration for the match.

`completionHandler`  

The block that GameKit calls when it completes the request.

This block receives the following parameters:

`match`  
The match that the players join. If unsuccessful, this parameter is `nil`.

`error`  
Describes an error if it occurs, or `nil` if the operation completes.

## Mentioned in 

Finding multiple players for a game

## Discussion

To find players using matchmaking rules, set the rules-related properties in `request` (queueName and optionally, properties) before you call this method. For more information, see Matchmaking rules.

## See Also

### Matching players

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

