

- GameKit
- GKAchievement
-  init(identifier:) 

Initializer

# init(identifier:)

Initializes an achievement for the local player.

iOS 4.1+iPadOS 4.1+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
init(identifier: String)
```

## Parameters 

`identifier`  

The identifier for the achievement that you enter in App Store Connect.

## Return Value

An achievement for a player, or `nil` if an error occurs.

## Mentioned in 

Rewarding players with achievements

## Discussion

Before creating an achievement, use the loadAchievements(completionHandler:) method to load the achievements that are in progress. If the achievement you want to report progress on isn’t in the array that GameKit passes to the handler, use this method to initialize the achievement.

## See Also

### Loading and Initializing Achievements

class func loadAchievements(completionHandler: (([GKAchievement]?, (any Error)?) -> Void)?)

Loads the achievements that you previously reported the player making progress toward.

init(identifier: String, player: GKPlayer)

Initializes an achievement for a player.

