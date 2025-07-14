

- GameKit
- GKTurnBasedMatch
-  find(for:withCompletionHandler:) 

Type Method

# find(for:withCompletionHandler:)

Creates a new match or finds an existing match that needs a player.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
class func find(
    for request: GKMatchRequest,
    withCompletionHandler completionHandler: @escaping (GKTurnBasedMatch?, (any Error)?) -> Void
)
```

``` source
class func find(for request: GKMatchRequest) async throws -> GKTurnBasedMatch
```

## Parameters 

`request`  

The configuration for the turn-based match.

`completionHandler`  

The block that GameKit calls when it completes the request.

The block receives the following parameters:

*match*  
A new or existing match, or `nil` if an error occurs.

*error*  
Describes an error if it occurs, or `nil` if the operation completes.

## Mentioned in 

Starting turn-based matches and passing turns between players

## Discussion

When you provide a custom interface for managing matches, use this method to programmatically create or find a turn-based match on behalf of the local player. The local player is always the current participant in the match object GameKit passes to the completion handler. Therefore, implement the completion handler to show the gameplay interface and let the local player take their turn.

To be consistent with older servers and earlier versions of iOS, GameKit sets the minimum number of players specified by the `GKMatchRequest` object to be equal to the maximum number of players when looking for a match.

## See Also

### Creating a Match

func acceptInvite(completionHandler: ((GKTurnBasedMatch?, (any Error)?) -> Void)?)

Accepts an invitation for the local player to join a turn-based match.

func declineInvite(completionHandler: (((any Error)?) -> Void)?)

Declines an invitation for the local player to join a turn-based match.

func rematch(completionHandler: ((GKTurnBasedMatch?, (any Error)?) -> Void)?)

Creates a new turn-based match with the same participants from an existing match.

