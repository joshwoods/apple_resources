

- GameKit
-  GKAccessPoint 

Class

# GKAccessPoint

An object that allows players to view and manage their Game Center information from within your game.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
class GKAccessPoint
```

## Mentioned in 

Adding an access point to your game

## Overview

The access point displays a control in a corner of your game that opens a Game Center dashboard when the player taps or clicks it.

Use the shared property to get the shared access point object. GameKit attaches the access point to the window you specify in the parentWindow property, in the corner you specify using the location property. If you don’t specify a parent window, GameKit infers an appropriate location. For the location of the access point on visionOS, see Configure the access point on visionOS.

To display highlights, set the showHighlights property to true. Then set isActive to true to display the access point control.

## Topics

### Getting the shared access point

class var shared: GKAccessPoint

The shared access point object.

### Managing the location

var location: GKAccessPoint.Location

The corner of the screen to display the access point.

enum Location

Specifies the corner of the screen to display the access point.

var frameInScreenCoordinates: CGRect

The frame of the access point in screen coordinates.

var parentWindow: UIWindow?

The window that contains the access point.

### Displaying the access point

var isActive: Bool

A Boolean value that determines whether to display the access point.

var isPresentingGameCenter: Bool

A Boolean value that indicates whether the game is presenting the Game Center dashboard.

var isVisible: Bool

A Boolean value that indicates whether the access point is visible.

var showHighlights: Bool

A Boolean value that indicates whether to display highlights for achievements and current ranks for leaderboards.

### Managing the access point

var isFocused: Bool

A Boolean value that indicates whether the access point is in focus on tvOS.

func trigger(handler: () -> Void)

Displays the Game Center dashboard as if the player taps or presses the access point.

func trigger(state: GKGameCenterViewControllerState, handler: () -> Void)

Displays the Game Center dashboard in the specified state as if the player taps or presses the access point.

func trigger(player: GKPlayer, handler: (() -> Void)?)

Displays the Game Center dashboard in a state that shows a player profile.

func trigger(achievementID: String, handler: (() -> Void)?)

Displays the Game Center dashboard in a state that shows a specific achievement.

func trigger(leaderboardID: String, playerScope: GKLeaderboard.PlayerScope, timeScope: GKLeaderboard.TimeScope, handler: (() -> Void)?)

Displays the Game Center dashboard in a state that shows a specific leaderboard.

func trigger(leaderboardSetID: String, handler: (() -> Void)?)

Displays the Game Center dashboard in a state that shows a specific leaderboard set.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Game Center interfaces

Adding an access point to your game

Provide your users a convenient connection to the Game Center dashboard.

Displaying the Game Center dashboard

Provide an interface for players to navigate to their Game Center data from your game.

class GKGameCenterViewController

The dashboard that allows players to access their Game Center data in your game.

class GKDialogController

An object that provides the ability to present the dashboard in macOS games.

protocol GKViewController

The abstract base protocol adopted by GameKit view controller classes.

class GKNotificationBanner

A Game Center-style banner that displays a message to the local player.

Deprecated

