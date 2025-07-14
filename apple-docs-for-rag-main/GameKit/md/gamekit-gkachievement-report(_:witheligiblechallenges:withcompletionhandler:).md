

- GameKit
- GKAchievement
-  report(\_:withEligibleChallenges:withCompletionHandler:) 

Type Method

# report(\_:withEligibleChallenges:withCompletionHandler:)

Reports the player’s progress on achievements and limits the challenges, associated with those achievements, that the player may complete.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
class func report(
    _ achievements: [GKAchievement],
    withEligibleChallenges challenges: [GKChallenge],
    withCompletionHandler completionHandler: (((any Error)?) -> Void)? = nil
)
```

``` source
class func report(
    _ achievements: [GKAchievement],
    withEligibleChallenges challenges: [GKChallenge]
) async throws
```

## Parameters 

`achievements`  

The achievements that you’re reporting to Game Center.

`challenges`  

The limited challenges associated with the achievements.

`completionHandler`  

A block that GameKit calls when this method completes.

The block receives the following parameter:

`error`  
Describes an error if it occurs, or `nil` if the operation completes.

## Discussion

Call this method to communicate to Game Center about the local player’s progress towards completing one or more achievements.

Game Center only updates the achievement’s percentComplete and lastReportedDate properties if the percentComplete property of an achievement that you pass to this method is greater than the current value. If the achievement is hidden, Game Center also makes it visible. If the percentComplete property is `100.0`, Game Center sets its isCompleted property to true and may show a banner to the player.

For efficiency, include multiple achievements rather than invoking this method separately for each achievement. Since Game Center associates an achievement with the local player at the time you create the achievement, only invoke this method after you authenticate the same player on the device.

## See Also

### Reporting Progress on Achievements

class func report([GKAchievement], withCompletionHandler: (((any Error)?) -> Void)?)

Reports the player’s progress of players toward one or more achievements.

var showsCompletionBanner: Bool

A Boolean value that indicates whether GameKit displays a banner when the player completes the achievement.

class func resetAchievements(completionHandler: (((any Error)?) -> Void)?)

Resets the percentage completed for all of the player’s achievements.

