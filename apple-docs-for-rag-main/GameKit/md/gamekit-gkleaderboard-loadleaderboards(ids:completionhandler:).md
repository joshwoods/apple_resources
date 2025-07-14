

- GameKit
- GKLeaderboard
-  loadLeaderboards(IDs:completionHandler:) 

Type Method

# loadLeaderboards(IDs:completionHandler:)

Loads leaderboards for the specified leaderboard IDs that Game Center uses.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
class func loadLeaderboards(
    IDs leaderboardIDs: [String]?,
    completionHandler: @escaping ([GKLeaderboard]?, (any Error)?) -> Void
)
```

``` source
class func loadLeaderboards(IDs leaderboardIDs: [String]?) async throws -> [GKLeaderboard]
```

## Parameters 

`leaderboardIDs`  

An array of leaderboard IDs that Game Center uses.

`completionHandler`  

A block that GameKit calls when this method loads the leaderboards.

The block receives the following parameters:

leaderboards  
The leaderboards that match the IDs.

error  
Describes an error if it occurs, or `nil` if the operation completes.

## Mentioned in 

Creating recurring leaderboards

Encourage progress and competition with leaderboards

## See Also

### Loading Leaderboards

func loadPreviousOccurrence(completionHandler: (GKLeaderboard?, (any Error)?) -> Void)

Loads the previous recurring leaderboard occurrence that the player submits a score to.

