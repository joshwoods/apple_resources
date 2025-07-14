

- GameKit
- GKAchievementDescription
-  rarityPercent 

Instance Property

# rarityPercent

The percentage of players of this game that earned the achievement.

iOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
var rarityPercent: Double? { get }
```

## Discussion

The rarity percentage ranges between `0.0` and `100.0`, inclusive, where `0.0` indicates that no player has earned the achievement, and `100.0` indicates that every player has earned the achievement. This property is `nil` if there isn’t enough data to compute the rarity of the achievement.

## See Also

### Reading and Writing Achievement Properties

var identifier: String

The string you enter in App Store Connect that uniquely identifies the achievement.

var title: String

A localized title for the achievement.

var unachievedDescription: String

A localized description of the achievement that you display when the player hasn’t completed the achievement.

var achievedDescription: String

A localized description of the achievement that you display when the player completes the achievement.

var maximumPoints: Int

The number of points that the player earns when completing the achievement.

var image: NSImage?

The achievement’s artwork that you display when the player completes the achievement.

Deprecated

var isHidden: Bool

A Boolean value that states whether the achievement is initially visible to players.

var isReplayable: Bool

A Boolean value that states whether the player can earn the achievement multiple times.

