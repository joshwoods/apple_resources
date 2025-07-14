

- GameKit
- GKLeaderboard
-  loadPreviousOccurrence(completionHandler:) 

Instance Method

# loadPreviousOccurrence(completionHandler:)

Loads the previous recurring leaderboard occurrence that the player submits a score to.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
func loadPreviousOccurrence(completionHandler: @escaping (GKLeaderboard?, (any Error)?) -> Void)
```

``` source
func loadPreviousOccurrence() async throws -> GKLeaderboard?
```

## Parameters 

`completionHandler`  

A block that GameKit calls when this method loads the leaderboard.

The block receives the following parameters:

leaderboard  
The previous occurrence of this leaderboard that the player submits a score to, or the most recent occurrence if GameKit can’t find the previous one.

error  
Describes an error if it occurs, or `nil` if the operation completes.

## Mentioned in 

Creating recurring leaderboards

Encourage progress and competition with leaderboards

## See Also

### Loading Leaderboards

class func loadLeaderboards(IDs: [String]?, completionHandler: ([GKLeaderboard]?, (any Error)?) -> Void)

Loads leaderboards for the specified leaderboard IDs that Game Center uses.

