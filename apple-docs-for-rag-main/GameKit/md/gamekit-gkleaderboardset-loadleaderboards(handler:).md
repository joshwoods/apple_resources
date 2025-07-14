

- GameKit
- GKLeaderboardSet
-  loadLeaderboards(handler:) 

Instance Method

# loadLeaderboards(handler:)

Loads the leaderboards in the leaderboard set.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
func loadLeaderboards(handler: @escaping ([GKLeaderboard]?, (any Error)?) -> Void)
```

## Parameters 

`handler`  

A block that GameKit calls when this method completes the request.

The block receives the following parameters:

*leaderboards*  
The leaderboards in the leaderboard set.

*error*  
Describes an error if it occurs, or `nil` if the operation completes.

## Mentioned in 

Encourage progress and competition with leaderboards

## See Also

### Loading Leaderboard Sets

func loadImage(completionHandler: ((UIImage?, (any Error)?) -> Void)?)

Loads the localized image that you associate with the leaderboard set.

class func loadLeaderboardSets(completionHandler: (([GKLeaderboardSet]?, (any Error)?) -> Void)?)

Loads all of the leaderboard sets you configure for your game.

func loadLeaderboards(completionHandler: (([GKLeaderboard]?, (any Error)?) -> Void)?)

Loads all of the leaderboards for the current leaderboard set.

Deprecated

