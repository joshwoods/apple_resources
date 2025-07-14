

- GameKit
- GKAchievement
-  resetAchievements(completionHandler:) 

Type Method

# resetAchievements(completionHandler:)

Resets the percentage completed for all of the player’s achievements.

iOS 4.1+iPadOS 4.1+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
class func resetAchievements(completionHandler: (((any Error)?) -> Void)? = nil)
```

``` source
class func resetAchievements() async throws
```

## Parameters 

`completionHandler`  

A block that GameKit calls when this method completes.

The block receives the following parameter:

`error`  
Describes an error if it occurs, or `nil` if the operation completes.

## Mentioned in 

Rewarding players with achievements

## Discussion

This method sets the percentage complete for all of the player’s achievements to zero. If you hide an achievement when you create it in App Store Connect, this method hides the achievement again.

## See Also

### Reporting Progress on Achievements

class func report([GKAchievement], withCompletionHandler: (((any Error)?) -> Void)?)

Reports the player’s progress of players toward one or more achievements.

class func report([GKAchievement], withEligibleChallenges: [GKChallenge], withCompletionHandler: (((any Error)?) -> Void)?)

Reports the player’s progress on achievements and limits the challenges, associated with those achievements, that the player may complete.

var showsCompletionBanner: Bool

A Boolean value that indicates whether GameKit displays a banner when the player completes the achievement.

