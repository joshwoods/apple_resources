

- GameKit
- GKAchievement
-  showsCompletionBanner 

Instance Property

# showsCompletionBanner

A Boolean value that indicates whether GameKit displays a banner when the player completes the achievement.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
var showsCompletionBanner: Bool { get set }
```

## Mentioned in 

Rewarding players with achievements

## Discussion

If this property is true, GameKit displays a notification banner to inform the player that they completed the achievement. If you want to present your own interface, set this property to false. The default value is true.

## See Also

### Reporting Progress on Achievements

class func report([GKAchievement], withCompletionHandler: (((any Error)?) -> Void)?)

Reports the player’s progress of players toward one or more achievements.

class func report([GKAchievement], withEligibleChallenges: [GKChallenge], withCompletionHandler: (((any Error)?) -> Void)?)

Reports the player’s progress on achievements and limits the challenges, associated with those achievements, that the player may complete.

class func resetAchievements(completionHandler: (((any Error)?) -> Void)?)

Resets the percentage completed for all of the player’s achievements.

