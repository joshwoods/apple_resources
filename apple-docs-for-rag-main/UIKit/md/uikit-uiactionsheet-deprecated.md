

- UIKit
-  UIActionSheet Deprecated

Class

# UIActionSheet

A view that presents a set of alternatives for how to proceed with a task.

iOS 2.0–8.3DeprecatediPadOS 2.0–8.3DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
class UIActionSheet
```

Deprecated

Instead, use UIAlertController with a preferredStyle of UIAlertController.Style.actionSheet.

## Overview

In apps that target versions of iOS prior to iOS 8, use the UIActionSheet class to present the user with a set of alternatives for how to proceed with a given task. You can also use action sheets to prompt the user to confirm a potentially dangerous action. The action sheet contains an optional title and one or more buttons, each of which corresponds to an action to take.

Use the properties and methods of this class to configure the action sheet’s message, style, and buttons before presenting it. You should also assign a delegate to your action sheet. Your delegate object is responsible for performing the action associated with any buttons when they’re tapped and should conform to the UIActionSheetDelegate protocol. For more information about implementing the methods of the delegate, see UIActionSheetDelegate.

You can present an action sheet from a toolbar, tab bar, button bar item, or from a view. This class takes the starting view and current platform into account when determining how to present the action sheet. For applications running on iPhone and iPod touch devices, the action sheet typically slides up from the bottom of the window that owns the view. For applications running on iPad devices, the action sheet is typically displayed in a popover that’s anchored to the starting view in an appropriate way. Taps outside of the popover automatically dismiss the action sheet, as do taps within any custom buttons. You can also dismiss it programmatically.

When presenting an action sheet on an iPad, there are times when you shouldn’t include a cancel button. If you’re presenting just the action sheet, the system displays the action sheet inside a popover without using an animation. Because taps outside the popover dismiss the action sheet without selecting an item, this results in a default way to cancel the sheet. Including a cancel button would therefore only cause confusion. However, if you have an existing popover and are displaying an action sheet on top of other content using an animation, a cancel button is still appropriate. For more information, see iOS Human Interface Guidelines.

Important

In iOS 4 and later, action sheets aren’t dismissed automatically when an application moves to the background. This behavior differs from earlier versions of the operating system, where action sheets were automatically canceled (and their cancellation handler executed) as part of the termination sequence for the application. Now, it’s up to you to decide whether to dismiss the action sheet (and execute its cancellation handler) or leave it visible for when your application moves back to the foreground. Remember that your application can still be terminated while in the background, so some type of action may be necessary in either case.

### Subclassing notes

UIActionSheet isn’t designed to be subclassed, nor should you add views to its hierarchy. If you need to present a sheet with more customization than provided by the UIActionSheet API, you can create your own and present it modally with present(_:animated:completion:).

## Topics

### Creating action sheets

convenience init(title: String?, delegate: (any UIActionSheetDelegate)?, cancelButtonTitle: String?, destructiveButtonTitle: String?, otherButtonTitles: String, String...)

Creates an action sheet with the specified values.

init(title: String?, delegate: (any UIActionSheetDelegate)?, cancelButtonTitle: String?, destructiveButtonTitle: String?)

Initializes the action sheet using the specified starting parameters.

### Setting properties

var delegate: (any UIActionSheetDelegate)?

The receiver’s delegate or `nil` if it doesn’t have a delegate.

var title: String

The string that appears in the receiver’s title bar.

var isVisible: Bool

A Boolean value that indicates whether the receiver is displayed.

var actionSheetStyle: UIActionSheetStyle

The receiver’s presentation style.

### Configuring buttons

func addButton(withTitle: String?) -> Int

Adds a custom button to the action sheet.

var numberOfButtons: Int

The number of buttons on the action sheet.

func buttonTitle(at: Int) -> String?

Returns the title of the button at the specified index.

var cancelButtonIndex: Int

The index number of the cancel button.

var destructiveButtonIndex: Int

The index number of the destructive button.

var firstOtherButtonIndex: Int

The index of the first custom button.

### Presenting the action sheet

func show(from: UITabBar)

Displays an action sheet that originates from the specified tab bar.

func show(from: UIToolbar)

Displays an action sheet that originates from the specified toolbar.

func show(in: UIView)

Displays an action sheet that originates from the specified view.

func show(from: UIBarButtonItem, animated: Bool)

Displays an action sheet that originates from the specified bar button item.

func show(from: CGRect, in: UIView, animated: Bool)

Displays an action sheet that originates from the specified view.

### Dismissing the action sheet

func dismiss(withClickedButtonIndex: Int, animated: Bool)

Dismisses the action sheet immediately using an optional animation.

### Constants

enum UIActionSheetStyle

Specifies the style of an action sheet.

## Relationships

### Inherits From

- UIView

### Conforms To

- CALayerDelegate
- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSTouchBarProvider
- Sendable
- UIAccessibilityIdentification
- UIActivityItemsConfigurationProviding
- UIAppearance
- UIAppearanceContainer
- UICoordinateSpace
- UIDynamicItem
- UIFocusEnvironment
- UIFocusItem
- UIFocusItemContainer
- UILargeContentViewerItem
- UIPasteConfigurationSupporting
- UIPopoverPresentationControllerSourceItem
- UIResponderStandardEditActions
- UITraitChangeObservable
- UITraitEnvironment
- UIUserActivityRestoring

## See Also

### Deprecated classes

class UIAlertView

A view that displays an alert message.

Deprecated

class UIDocumentMenuViewController

A list of all the available document providers for a given file type and mode, in addition to custom menu items that you add.

Deprecated

class UILocalNotification

A notification that an app can schedule for presentation at a specific date and time.

Deprecated

class UIMenuController

The menu interface for the Cut, Copy, Paste, Select, Select All, and Delete commands.

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

