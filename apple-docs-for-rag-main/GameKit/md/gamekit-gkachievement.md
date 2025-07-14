

- GameKit
-  GKAchievement 

Class

# GKAchievement

An achievement you can award a player as they make progress toward and reach a goal in your game.

iOS 4.1+iPadOS 4.1+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
class GKAchievement
```

## Mentioned in 

Rewarding players with achievements

## Overview

Before using this class, configure your game achievements in App Store Connect. Then the dashboard shows the achievements initially locked and you can access them in your code.

Use the loadAchievements(completionHandler:) method to load all the achievements that the local player is progressing toward. If an achievement doesn’t load, then it’s the first time you’re reporting the player’s progress toward it, and you must create a GKAchievement object to represent it. Next, set the percentage complete of the achievement using the percentComplete property.

You can report the player’s progress for one or more achievements to Game Center using the report(_:withCompletionHandler:) method. The dashboard changes the appearance of the achievements to show the current percentages. If you set the percentage of an achievement to 100, the dashboard shows it as completed.

To reset the player’s progress on all achievements, use the resetAchievements(completionHandler:) class method.

## Topics

### Loading and Initializing Achievements

class func loadAchievements(completionHandler: (([GKAchievement]?, (any Error)?) -> Void)?)

Loads the achievements that you previously reported the player making progress toward.

init(identifier: String)

Initializes an achievement for the local player.

init(identifier: String, player: GKPlayer)

Initializes an achievement for a player.

### Accessing Achievement Properties

var identifier: String

The identifier for the achievement that you enter in App Store Connect.

var player: GKPlayer

The player who earned the achievement.

var percentComplete: Double

A percentage value that states how far the player has progressed on the achievement.

var isCompleted: Bool

A Boolean value that states whether the player has completed the achievement.

var lastReportedDate: Date

The last time your game reported progress on the achievement for the player.

### Reporting Progress on Achievements

class func report([GKAchievement], withCompletionHandler: (((any Error)?) -> Void)?)

Reports the player’s progress of players toward one or more achievements.

class func report([GKAchievement], withEligibleChallenges: [GKChallenge], withCompletionHandler: (((any Error)?) -> Void)?)

Reports the player’s progress on achievements and limits the challenges, associated with those achievements, that the player may complete.

var showsCompletionBanner: Bool

A Boolean value that indicates whether GameKit displays a banner when the player completes the achievement.

class func resetAchievements(completionHandler: (((any Error)?) -> Void)?)

Resets the percentage completed for all of the player’s achievements.

### Issuing Achievement Challenges

func selectChallengeablePlayers([GKPlayer], withCompletionHandler: (([GKPlayer]?, (any Error)?) -> Void)?)

Finds the subset of players who can earn an achievement.

func challengeComposeController(withMessage: String?, players: [GKPlayer], completion: GKChallengeComposeHandler?) -> UIViewController

Provides a view controller that you present to the player to issue an achievement challenge.

typealias GKChallengeComposeHandler

A completion block that provides information about the player who issues a challenge and the players who receive it.

func challengeComposeController(withMessage: String?, players: [GKPlayer], completionHandler: GKChallengeComposeCompletionBlock?) -> UIViewController

Provides a view controller that you present to the player to issue an achievement challenge.

Deprecated

func challengeComposeController(withPlayers: [String]?, message: String?, completionHandler: GKChallengeComposeCompletionBlock?) -> UIViewController?

Provides a challenge compose view controller with preselected player identifiers and a message.

Deprecated

### Deprecated

Deprecated Symbols

Review unsupported symbols and their replacements.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding
- Sendable

## See Also

### Achievements

Rewarding players with achievements

Use achievements to motivate players and engage them more in your game.

class GKAchievementDescription

An object containing the text and artwork used to present an achievement to a player.

