

- GameKit
- GKLeaderboardSet
-  loadLeaderboardSets(completionHandler:) 

Type Method

# loadLeaderboardSets(completionHandler:)

Loads all of the leaderboard sets you configure for your game.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
class func loadLeaderboardSets(completionHandler: (([GKLeaderboardSet]?, (any Error)?) -> Void)? = nil)
```

``` source
class func loadLeaderboardSets() async throws -> [GKLeaderboardSet]
```

## Parameters 

`completionHandler`  

A block that GameKit calls when this method completes the request.

The block receives the following parameters:

*leaderboardSets*  
The leaderboard sets in your game.

*error*  
Describes an error if it occurs, or `nil` if the operation completes.

## Mentioned in 

Encourage progress and competition with leaderboards

## See Also

### Loading Leaderboard Sets

func loadImage(completionHandler: ((UIImage?, (any Error)?) -> Void)?)

Loads the localized image that you associate with the leaderboard set.

func loadLeaderboards(handler: ([GKLeaderboard]?, (any Error)?) -> Void)

Loads the leaderboards in the leaderboard set.

func loadLeaderboards(completionHandler: (([GKLeaderboard]?, (any Error)?) -> Void)?)

Loads all of the leaderboards for the current leaderboard set.

Deprecated

