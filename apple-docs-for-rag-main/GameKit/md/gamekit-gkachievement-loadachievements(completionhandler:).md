

- GameKit
- GKAchievement
-  loadAchievements(completionHandler:) 

Type Method

# loadAchievements(completionHandler:)

Loads the achievements that you previously reported the player making progress toward.

iOS 4.1+iPadOS 4.1+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
class func loadAchievements(completionHandler: (([GKAchievement]?, (any Error)?) -> Void)? = nil)
```

``` source
class func loadAchievements() async throws -> [GKAchievement]
```

## Parameters 

`completionHandler`  

A block that GameKit calls when this method loads the achievements.

The block receives the following parameters:

`achievements`  
The achievements that you previously reported progress for the local player.

`error`  
Describes an error if it occurs, or `nil` if the operation completes.

## Mentioned in 

Rewarding players with achievements

## See Also

### Loading and Initializing Achievements

init(identifier: String)

Initializes an achievement for the local player.

init(identifier: String, player: GKPlayer)

Initializes an achievement for a player.

