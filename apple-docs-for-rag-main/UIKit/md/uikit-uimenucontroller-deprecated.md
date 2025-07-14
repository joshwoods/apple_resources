

- UIKit
-  UIMenuController Deprecated

Class

# UIMenuController

The menu interface for the Cut, Copy, Paste, Select, Select All, and Delete commands.

iOS 3.0–16.0DeprecatediPadOS 3.0–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
@MainActor
class UIMenuController
```

Deprecated

Use UIEditMenuInteraction instead.

## Overview

The singleton UIMenuController instance is referred to as the editing menu. When you make this menu visible, UIMenuController positions it relative to a target rectangle on the screen; this rectangle usually defines a selection. The menu appears above the target rectangle or, if there isn’t enough space for it, below it. The menu’s pointer is placed at the center of the top or bottom of the target rectangle, as appropriate. Be sure to set the tracking rectangle before you make the menu visible. You’re also responsible for detecting, tracking, and displaying selections.

The UIResponderStandardEditActions informal protocol declares methods that are invoked when the user taps a menu command. The canPerformAction(_:withSender:) method of UIResponder is also related to the editing menu. A responder implements this method to enable and disable commands of the editing menu just before the menu is displayed. You can force the menu commands enabled state to update by calling the update() method.

You can also provide your own menu items via the menuItems property. When you modify the menu items, you can use the update() method to force the menu to update its display.

## Topics

### Getting the menu controller instance

class var shared: UIMenuController

Returns the menu controller.

### Showing and hiding the menu

func showMenu(from: UIView, rect: CGRect)

func hideMenu(from: UIView)

func hideMenu()

var isMenuVisible: Bool

The visibility of the editing menu.

func setMenuVisible(Bool, animated: Bool)

Shows or hides the editing menu, optionally animating the action.

### Positioning the menu

var menuFrame: CGRect

Returns the frame of the editing menu.

var arrowDirection: UIMenuController.ArrowDirection

The direction the arrow of the editing menu is pointing.

enum ArrowDirection

The direction the arrow of the editing menu is pointing.

func setTargetRect(CGRect, in: UIView)

Sets the area in a view above or below which the editing menu is positioned.

### Updating the menu

func update()

Updates the appearance and enabled state of menu commands.

### Customizing menu items

var menuItems: [UIMenuItem]?

The custom menu items for the editing menu.

### Notifications

class let willShowMenuNotification: NSNotification.Name

Posted by the menu controller just before it shows the menu.

class let didShowMenuNotification: NSNotification.Name

Posted by the menu controller just after it shows the menu.

class let willHideMenuNotification: NSNotification.Name

Posted by the menu controller just before it hides the menu.

class let didHideMenuNotification: NSNotification.Name

Posted by the menu controller just after it hides the menu.

class let menuFrameDidChangeNotification: NSNotification.Name

Posted when the frame of a visible menu changes.

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
- Sendable

## See Also

### Deprecated classes

class UIActionSheet

A view that presents a set of alternatives for how to proceed with a task.

Deprecated

class UIAlertView

A view that displays an alert message.

Deprecated

class UIDocumentMenuViewController

A list of all the available document providers for a given file type and mode, in addition to custom menu items that you add.

Deprecated

class UILocalNotification

A notification that an app can schedule for presentation at a specific date and time.

Deprecated

class UIMenuItem

A custom item in the editing menu managed by the menu controller.

Deprecated

class UIMutableUserNotificationAction

A modifiable version of the user notification action class.

Deprecated

class UIMutableUserNotificationCategory

Information about custom actions that your app can perform in response to a local or push notification.

Deprecated

class UIPopoverController

An object that manages the presentation of content in a popover.

Deprecated

class UIPreviewAction

A preview action, or *peek quick action*, that displays below a peek when a user swipes the peek upward.

Deprecated

class UIPreviewActionGroup

A group of one or more child quick actions, each an instance of the preview action class.

Deprecated

class UISearchDisplayController

An object that manages the display of a search bar, along with a table view that displays search results.

Deprecated

class UIStoryboardPopoverSegue

A specific type of segue for presenting content in a popover.

Deprecated

class UIUserNotificationAction

A custom action that your app can perform in response to a remote or local notification.

Deprecated

class UIUserNotificationCategory

Information about custom actions that your app can perform in response to a local or push notification.

Deprecated

class UIUserNotificationSettings

The types of notifications that can be displayed to the user by your app.

Deprecated

