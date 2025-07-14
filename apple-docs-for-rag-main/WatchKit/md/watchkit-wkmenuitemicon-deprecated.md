

- WatchKit
-  WKMenuItemIcon Deprecated

Enumeration

# WKMenuItemIcon

Template images that you can use for menus.

watchOS 2.0–7.0Deprecated

``` source
enum WKMenuItemIcon
```

Deprecated

Elevate important items out of such menus and into the relevant screen or a settings screen.

## Overview

Use these constants with the addMenuItem(with:title:action:) method to configure actions for your interface controller’s menu.

## Topics

### Constants

case accept

The icon indicating an action to accept an event or item.

case add

The icon indicating an action for adding an item.

case block

The icon indicating an action to block or prevent something from happening.

case decline

The icon indicating an action to decline or cancel an event.

case info

The icon indicating an action to retrieve more information.

case maybe

The icon indicating an answer of maybe for an action.

case more

The icon indicating that more actions or options are available.

case mute

The icon indicating an action to mute the sound.

case pause

The icon indicating an action to pause playback.

case play

The icon indicating an action to play some content.

case `repeat`

The icon indicating that played content should repeat in a loop.

case resume

The icon indicating an action to resume playing some content.

case share

The icon indicating an action to share content.

case shuffle

The icon indicating an action to shuffle content.

case speaker

The icon indicating audio output.

case trash

The icon indicating an action to delete some content.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Deprecated symbols

Text Response Key

Keys for retrieving text response information.

func addMenuItem(withImageNamed: String, title: String, action: Selector)

Adds an action to the context menu using an existing image resource in your Watch app bundle.

Deprecated

func addMenuItem(with: WKMenuItemIcon, title: String, action: Selector)

Adds an action to the context menu using a system-provided icon.

Deprecated

func addMenuItem(with: UIImage, title: String, action: Selector)

Adds an action to the context menu by using an image provided by your WatchKit extension.

Deprecated

func beginGlanceUpdates()

Tells the system that you are about to start a potentially lengthy update task for your glance.

Deprecated

func clearAllMenuItems()

Removes all programmatically added actions from the context menu.

Deprecated

func endGlanceUpdates()

Tells the system that you finished updating your glance content.

Deprecated

func handleUserActivity([AnyHashable : Any]?)

Responds to Handoff–related activity.

Deprecated

func presentController([(name: String, context: AnyObject)])

Presents a page-based interface modally.

Deprecated

class func reloadRootControllers(withNames: [String], contexts: [Any]?)

Loads the specified interface controllers and rebuilds the app’s page-based interface.

Deprecated

func updateUserActivity(String, userInfo: [AnyHashable : Any]?, webpageURL: URL?)

Registers the current user activity with the system.

Deprecated

