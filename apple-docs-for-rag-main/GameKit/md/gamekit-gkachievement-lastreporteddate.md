

- GameKit
- GKAchievement
-  lastReportedDate 

Instance Property

# lastReportedDate

The last time your game reported progress on the achievement for the player.

iOS 4.1+iPadOS 4.1+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
var lastReportedDate: Date { get }
```

## Discussion

GameKit initializes this property to the current date.

## See Also

### Accessing Achievement Properties

var identifier: String

The identifier for the achievement that you enter in App Store Connect.

var player: GKPlayer

The player who earned the achievement.

var percentComplete: Double

A percentage value that states how far the player has progressed on the achievement.

var isCompleted: Bool

A Boolean value that states whether the player has completed the achievement.

