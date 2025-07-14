

- GameKit
- GKTurnBasedMatch
-  declineInvite(completionHandler:) 

Instance Method

# declineInvite(completionHandler:)

Declines an invitation for the local player to join a turn-based match.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
func declineInvite(completionHandler: (((any Error)?) -> Void)? = nil)
```

``` source
func declineInvite() async throws
```

## Parameters 

`completionHandler`  

The block that GameKit calls when it completes the request.

The block receives the following parameter:

*error*  
Describes an error if it occurs, or `nil` if the operation completes.

## Mentioned in 

Starting turn-based matches and passing turns between players

## Discussion

When you provide a custom interface for managing matches, use this method to programmatically decline an invitation on behalf of the local player.

## See Also

### Creating a Match

class func find(for: GKMatchRequest, withCompletionHandler: (GKTurnBasedMatch?, (any Error)?) -> Void)

Creates a new match or finds an existing match that needs a player.

func acceptInvite(completionHandler: ((GKTurnBasedMatch?, (any Error)?) -> Void)?)

Accepts an invitation for the local player to join a turn-based match.

func rematch(completionHandler: ((GKTurnBasedMatch?, (any Error)?) -> Void)?)

Creates a new turn-based match with the same participants from an existing match.

