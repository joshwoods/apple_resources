

- GameKit
- GKTurnBasedMatch
-  remove(completionHandler:) 

Instance Method

# remove(completionHandler:)

Removes a match from Game Center that the local player participants in.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
func remove(completionHandler: (((any Error)?) -> Void)? = nil)
```

``` source
func remove() async throws
```

## Parameters 

`completionHandler`  

The block that GameKit calls when it completes the request.

The block receives the following parameter:

*error*  
Describes an error if it occurs, or `nil` if the operation completes.

## Discussion

If you don’t use the GKTurnBasedMatchmakerViewController interface, where players can delete their matches, use this method to delete a match that the local player no longer actively participants in. This method only removes the match from the local player’s Game Center data — it doesn’t impact other participants in the match.

