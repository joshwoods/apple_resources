

- GameKit
- GKLeaderboardScore
-  context 

Instance Property

# context

An integer value that your game uses.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
var context: Int { get set }
```

## Discussion

Game Center stores this custom game-specific property for you. It allows you to associate an arbitrary 64-bit unsigned integer value with the score data that you report to Game Center. You decide how to interpret this integer value in your game.

## See Also

### Accessing Properties

var leaderboardID: String

The ID that Game Center uses for the leaderboard.

var player: GKPlayer

The player who earns the score.

var value: Int

The score that the player earns.

