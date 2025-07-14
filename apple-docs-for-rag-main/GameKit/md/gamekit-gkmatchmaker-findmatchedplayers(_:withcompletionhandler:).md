

- GameKit
- GKMatchmaker
-  findMatchedPlayers(\_:withCompletionHandler:) 

Instance Method

# findMatchedPlayers(\_:withCompletionHandler:)

Initiates a request to find players for a hosted match that uses matchmaking rules.

iOS 17.2+iPadOS 17.2+Mac Catalyst 17.2+macOS 14.2+tvOS 17.2+visionOS 1.1+

``` source
func findMatchedPlayers(
    _ request: GKMatchRequest,
    withCompletionHandler completionHandler: @escaping (GKMatchedPlayers?, (any Error)?) -> Void
)
```

``` source
func findMatchedPlayers(_ request: GKMatchRequest) async throws -> GKMatchedPlayers
```

## Parameters 

`request`  

The configuration for the match.

`completionHandler`  

The block that GameKit calls when it completes the request.

This block receives the following parameters:

`matchedPlayers`  
The players that join the match, including their properties that matchmaking rules uses. If unsuccessful, this parameter is `nil`.

`error`  
Describes an error if it occurs, or `nil` if the operation completes.

## Discussion

To find players using matchmaking rules, set the rules-related properties in `request` (queueName and optionally, properties) before you call this method. For more information, see Matchmaking rules.

## See Also

### Matching players

func findMatch(for: GKMatchRequest, withCompletionHandler: ((GKMatch?, (any Error)?) -> Void)?)

Initiates a request to find players for a peer-to-peer match.

func findPlayers(forHostedRequest: GKMatchRequest, withCompletionHandler: (([GKPlayer]?, (any Error)?) -> Void)?)

Initiates a request to find players for a hosted match.

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

