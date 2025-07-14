

- GameKit
- GKLeaderboard
-  submitScore(\_:context:player:completionHandler:) 

Instance Method

# submitScore(\_:context:player:completionHandler:)

Submits a score to the leaderboard.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
func submitScore(
    _ score: Int,
    context: Int,
    player: GKPlayer,
    completionHandler: @escaping ((any Error)?) -> Void
)
```

``` source
func submitScore(
    _ score: Int,
    context: Int,
    player: GKPlayer
) async throws
```

## Parameters 

`score`  

The score that the player earns.

`context`  

An integer value that your game uses.

`player`  

The player who earns the score.

`completionHandler`  

A block that GameKit calls when this method adds the score.

The block receives the following parameters:

error  
Describes an error if it occurs, or `nil` if the operation completes.

## Mentioned in 

Creating recurring leaderboards

Encourage progress and competition with leaderboards

## See Also

### Submitting Scores

class func submitScore(Int, context: Int, player: GKPlayer, leaderboardIDs: [String], completionHandler: ((any Error)?) -> Void)

Submits a score to multiple leaderboards.

