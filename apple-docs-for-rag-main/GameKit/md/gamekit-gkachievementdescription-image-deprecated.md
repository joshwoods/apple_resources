

- GameKit
- GKAchievementDescription
-  image Deprecated

Instance Property

# image

The achievement’s artwork that you display when the player completes the achievement.

macOS 10.8–14.2DeprecatedtvOS 9.0–17.2DeprecatedvisionOS 1.0–1.0Deprecated

**tvOS, visionOS**

``` source
var image: UIImage? { get }
```

**macOS**

``` source
var image: NSImage? { get }
```

## Discussion

The value of this property is undefined until you load the image using the loadImage(completionHandler:) method.

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

var isHidden: Bool

A Boolean value that states whether the achievement is initially visible to players.

var isReplayable: Bool

A Boolean value that states whether the player can earn the achievement multiple times.

var rarityPercent: Double?

The percentage of players of this game that earned the achievement.

