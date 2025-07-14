

- WebKit
- WKWebExtension
-  WKWebExtension.Action 

Class

# WKWebExtension.Action

An object that encapsulates the properties for an individual web extension action.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
class Action
```

## Overview

This class provides access to action properties, such as pop-up, icon, or title, with tab-specific values.

## Topics

### Instance Properties

var associatedTab: (any WKWebExtensionTab)?

The tab that this action is associated with, or `nil` if it’s the default action.

var badgeText: String

The badge text for the action.

var hasUnreadBadgeText: Bool

A Boolean value indicating whether the badge text is unread.

var inspectionName: String?

The name shown when inspecting the pop-up web view.

var isEnabled: Bool

A Boolean value indicating whether the action is enabled.

var label: String

The localized display label for the action.

var menuItems: [UIMenuElement]

The menu items provided by the extension for this action.

var popupPopover: NSPopover?

A popover that presents a web view loaded with the pop-up page for this action, or `nil` if no popup is specified.

var popupViewController: UIViewController?

A view controller that presents a web view loaded with the pop-up page for this action, or `nil` if no popup is specified.

var popupWebView: WKWebView?

A web view loaded with the pop-up page for this action, or `nil` if no pop-up is specified.

var presentsPopup: Bool

A Boolean value indicating whether the action has a pop-up.

var webExtensionContext: WKWebExtensionContext?

The extension context to which this action is related.

### Instance Methods

func closePopup()

Triggers the dismissal process of the pop-up.

func icon(for: CGSize) -> UIImage?

Returns the action icon for the specified size.

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

### Classes

class Command

An object that encapsulates the properties for an individual web extension command.

class DataRecord

An object that represents a record of stored data for a specific web extension context.

class MatchPattern

An object that represents a way to specify groups of URLs.

class MessagePort

An object that manages message-based communication with a web extension.

class TabConfiguration

An object that encapsulates configuration options for a tab in an extension.

class WindowConfiguration

An object that encapsulates configuration options for a window in an extension.

class Configuration

A WKWebExtensionController.Configuration object with which to initialize a web extension controller.

