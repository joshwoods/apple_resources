

- GameKit
- GKAchievementDescription
-  isHidden 

Instance Property

# isHidden

A Boolean value that states whether the achievement is initially visible to players.

iOS 4.1+iPadOS 4.1+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
var isHidden: Bool { get }
```

## Discussion

If the value of this property is false, the achievement is always visible to the player. If true, the achievement isn’t displayed in any of the standard achievement user interface screens. It remains hidden until the first time your game reports progress toward completing the achievement.

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

var isReplayable: Bool

A Boolean value that states whether the player can earn the achievement multiple times.

var rarityPercent: Double?

The percentage of players of this game that earned the achievement.

