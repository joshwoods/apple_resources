

- GameKit
-  GKDialogController 

Class

# GKDialogController

An object that provides the ability to present the dashboard in macOS games.

macOS 10.8+

``` source
@MainActor
class GKDialogController
```

## Overview

For macOS games, use a `GKDialogController` object to present the dashboard from which players can browse and manage their Game Center data.

Initialize a new GKGameCenterViewController object, as you would for an iOS game, specifying the state and setting its delegate. Then get the singleton dialog controller using the shared() class method, or initialize a new `GKDialogController` object.

To present the dashboard, set the parentWindow property to the window that should display the dashboard and then call the present(_:) method, passing the `GKGameCenterViewController` object.

```
func presentAchievement() {
    let viewController = GKGameCenterViewController(achievementID: "101")
    viewController.gameCenterDelegate = self

    let dialogController = GKDialogController.shared()
    dialogController.parentWindow = NSApplication.shared.mainWindow
    dialogController.present(viewController)
}
```

When the player closes the dashboard, GameKit calls the gameCenterViewControllerDidFinish(_:) delegate method. Implement this method to dismiss the shared dialog controller using the dismiss(_:) method.

```
func gameCenterViewControllerDidFinish(_ gameCenterViewController: GKGameCenterViewController) {
    // Dismiss the view controller.
    let dialogController = GKDialogController.shared()
    dialogController.dismiss(self)
}
```

## Topics

### Accessing the Shared Dialog Controller

class func shared() -> GKDialogController

Retrieves the shared instance of the dialog controller.

### Setting the Presentation Window

var parentWindow: NSWindow?

The window that displays the dashboard.

### Presenting and Dismissing the Dialog

func present(any NSViewController &amp; GKViewController) -> Bool

Presents the dashboard in the window.

func dismiss(Any)

Dismisses the dashboard.

## Relationships

### Inherits From

- NSResponder

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSStandardKeyBindingResponding
- NSTouchBarProvider
- NSUserActivityRestoring
- Sendable

## See Also

### Game Center interfaces

Adding an access point to your game

Provide your users a convenient connection to the Game Center dashboard.

Displaying the Game Center dashboard

Provide an interface for players to navigate to their Game Center data from your game.

class GKAccessPoint

An object that allows players to view and manage their Game Center information from within your game.

class GKGameCenterViewController

The dashboard that allows players to access their Game Center data in your game.

protocol GKViewController

The abstract base protocol adopted by GameKit view controller classes.

class GKNotificationBanner

A Game Center-style banner that displays a message to the local player.

Deprecated

