

- GameKit
-  GKNotificationBanner Deprecated

Class

# GKNotificationBanner

A Game Center-style banner that displays a message to the local player.

iOS 5.0–17.0DeprecatediPadOS 5.0–17.0DeprecatedMac Catalyst 13.1–17.0DeprecatedmacOS 10.8–14.0DeprecatedtvOS 9.0–16.1DeprecatedvisionOS 1.0–1.0Deprecated

``` source
class GKNotificationBanner
```

Deprecated

Use UNNotificationRequest or provide a custom interface instead.

## Overview

This class displays a message in a banner to the local player, similar to the banner that GameKit displays when a player earns an achievement. If the game is in the foreground, the banner appears immediately. If the game is in the background, the banner appears when the game becomes active.

To display the banner with your message, use the show(withTitle:message:completionHandler:) method. To specify a duration that GameKit presents the banner, use the show(withTitle:message:duration:completionHandler:) method instead. Optionally, pass these methods a completion handler that GameKit calls after it dismisses the banner.

```
GKNotificationBanner.show(withTitle:"Hooray",
                          message:"You passed level 1 and can move to level 2.",
                          completionHandler: nil)
```

## Topics

### Displaying the Banner

class func show(withTitle: String?, message: String?, completionHandler: (() -> Void)?)

Displays a banner with a title and message to the player.

class func show(withTitle: String?, message: String?, duration: TimeInterval, completionHandler: (() -> Void)?)

Displays a banner to the player for a specified period of time.

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

class GKAccessPoint

An object that allows players to view and manage their Game Center information from within your game.

class GKGameCenterViewController

The dashboard that allows players to access their Game Center data in your game.

class GKDialogController

An object that provides the ability to present the dashboard in macOS games.

protocol GKViewController

The abstract base protocol adopted by GameKit view controller classes.

