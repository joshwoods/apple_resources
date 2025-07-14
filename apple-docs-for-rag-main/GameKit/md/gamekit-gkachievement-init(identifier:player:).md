

- GameKit
- GKAchievement
-  init(identifier:player:) 

Initializer

# init(identifier:player:)

Initializes an achievement for a player.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
init(
    identifier: String,
    player: GKPlayer
)
```

## Parameters 

`identifier`  

The identifier for the achievement that you enter in App Store Connect.

`player`  

The player who is earning the achievement.

## Return Value

An achievement for a player, or `nil` if an error occurs.

## Mentioned in 

Rewarding players with achievements

## Discussion

Before creating an achievement, use the loadAchievements(completionHandler:) method to load the achievements that are in progress. If the achievement you want to report progress on isn’t in the array that GameKit passes to the handler, use this method to initialize the achievement, but only when reporting progress for a participant at the end of a turn-based match. Otherwise, use the init(identifier:) method to initialize the achievement.

## See Also

### Loading and Initializing Achievements

class func loadAchievements(completionHandler: (([GKAchievement]?, (any Error)?) -> Void)?)

Loads the achievements that you previously reported the player making progress toward.

init(identifier: String)

Initializes an achievement for the local player.

