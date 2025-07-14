

- GameKit
- GKLeaderboardSet
-  loadLeaderboards(completionHandler:) Deprecated

Instance Method

# loadLeaderboards(completionHandler:)

Loads all of the leaderboards for the current leaderboard set.

iOS 7.0–14.0DeprecatediPadOS 7.0–14.0DeprecatedMac Catalyst 13.1–14.0DeprecatedmacOS 10.10–11.0DeprecatedtvOS 9.0–14.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–7.0Deprecated

``` source
func loadLeaderboards(completionHandler: (([GKLeaderboard]?, (any Error)?) -> Void)? = nil)
```

``` source
func loadLeaderboards() async throws -> [GKLeaderboard]
```

Deprecated

Use loadLeaderboards(handler:) instead.

## Parameters 

`completionHandler`  

A block that this method calls when it loads the leaderboards.

The block receives the following parameters:

*leaderboards*  
An array of `GKLeaderboard` objects that provides the leaderboards for your game.

*error*  
Describes an error if it occurs, or `nil` if the operation completes.

## See Also

### Loading Leaderboard Sets

func loadImage(completionHandler: ((UIImage?, (any Error)?) -> Void)?)

Loads the localized image that you associate with the leaderboard set.

class func loadLeaderboardSets(completionHandler: (([GKLeaderboardSet]?, (any Error)?) -> Void)?)

Loads all of the leaderboard sets you configure for your game.

func loadLeaderboards(handler: ([GKLeaderboard]?, (any Error)?) -> Void)

Loads the leaderboards in the leaderboard set.

