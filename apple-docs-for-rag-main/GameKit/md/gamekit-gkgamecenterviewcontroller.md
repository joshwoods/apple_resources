

- GameKit
-  GKGameCenterViewController 

Class

# GKGameCenterViewController

The dashboard that allows players to access their Game Center data in your game.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
class GKGameCenterViewController
```

## Mentioned in 

Displaying the Game Center dashboard

Adding an access point to your game

## Overview

This view controller presents the dashboard from which players can browse and manage their Game Center data. You can present the dashboard in a specific state from which players can navigate to other areas, including their profile. Your game should pause other activities before presenting the dashboard.

To present the dashboard, initialize a new GKGameCenterViewController object and set its delegate. Optionally, initialize a view controller in a specific state, to show a leaderboard with scores from a set of players or during a time period, or to show a specific achievement. Then present the view controller to the player, and GameKit calls your delegate when the player dismisses it.

For visionOS games, the dashboard appears anchored to the window, scene, or view relative to where you present the view controller. For immersive games, set the parent window to a separate window group than the immersive space window group. For the visionOS location of the dashboard when using the access point, see Configure the access point on visionOS.

## Topics

### Configuring Game Center content

init(state: GKGameCenterViewControllerState)

Creates a view controller that presents the specified Game Center content.

enum GKGameCenterViewControllerState

The type of content for the view controller to present.

init(leaderboard: GKLeaderboard, playerScope: GKLeaderboard.PlayerScope)

Creates a view controller that presents a leaderboard with data for the specified players.

init(leaderboardID: String, playerScope: GKLeaderboard.PlayerScope, timeScope: GKLeaderboard.TimeScope)

Creates a view controller that presents a leaderboard with data from the specified players and time period.

init(leaderboardSetID: String)

Creates a view controller that presents a leaderboard set.

init(achievementID: String)

Creates a view controller that presents an achievement.

init(player: GKPlayer)

Creates a view controller that presents a player’s Game Center profile.

### Setting the view controller delegate

var gameCenterDelegate: (any GKGameCenterControllerDelegate)?

The view controller’s delegate.

protocol GKGameCenterControllerDelegate

The delegate that GameKit calls when the player dismisses the dashboard.

### Deprecated

Deprecated Symbols

Review unsupported symbols and their replacements.

## Relationships

### Inherits From

- NSViewController
- UINavigationController

### Inherited By

- GKAchievementViewController
- GKLeaderboardViewController

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- GKViewController
- Hashable
- NSCoding
- NSEditor
- NSExtensionRequestHandling
- NSObjectProtocol
- NSSeguePerforming
- NSStandardKeyBindingResponding
- NSTouchBarProvider
- NSUserActivityRestoring
- NSUserInterfaceItemIdentification
- Sendable
- UIActivityItemsConfigurationProviding
- UIAppearanceContainer
- UIContentContainer
- UIFocusEnvironment
- UIPasteConfigurationSupporting
- UIResponderStandardEditActions
- UIStateRestoring
- UITraitChangeObservable
- UITraitEnvironment
- UIUserActivityRestoring

## See Also

### Game Center interfaces

Adding an access point to your game

Provide your users a convenient connection to the Game Center dashboard.

Displaying the Game Center dashboard

Provide an interface for players to navigate to their Game Center data from your game.

class GKAccessPoint

An object that allows players to view and manage their Game Center information from within your game.

class GKDialogController

An object that provides the ability to present the dashboard in macOS games.

protocol GKViewController

The abstract base protocol adopted by GameKit view controller classes.

class GKNotificationBanner

A Game Center-style banner that displays a message to the local player.

Deprecated

