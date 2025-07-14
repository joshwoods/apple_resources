

- WebKit
-  WKWebExtensionContext 

Class

# WKWebExtensionContext

An object that represents the runtime environment for a web extension.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
class WKWebExtensionContext
```

## Overview

This class provides methods for managing the extension’s permissions, allowing it to inject content, run background logic, show popovers, and display other web-based UI to the user.

## Topics

### Enumerations

enum PermissionStatus

Constants used to indicate permission status in web extension context.

### Structures

struct Error

Constants used to indicate errors in the web extension context domain.

struct NotificationUserInfoKey

Constants for specifying web extension context information in notifications.

### Initializers

init(for: WKWebExtension)

Returns a web extension context initialized with a specified extension.

### Instance Properties

var baseURL: URL

The base URL the context uses for loading extension resources or injecting content into webpages.

var commands: [WKWebExtension.Command]

The commands associated with the extension.

var currentPermissionMatchPatterns: Set&lt;WKWebExtension.MatchPattern>

The currently granted permission match patterns that have not expired.

var currentPermissions: Set&lt;WKWebExtension.Permission>

The currently granted permissions that have not expired.

var deniedPermissionMatchPatterns: [WKWebExtension.MatchPattern : Date]

The currently denied permission match patterns and their expiration dates.

var deniedPermissions: [WKWebExtension.Permission : Date]

The currently denied permissions and their expiration dates.

var errors: [any Error]

All errors that occurred in the extension context.

var focusedWindow: (any WKWebExtensionWindow)?

The window that currently has focus for this extension.

var grantedPermissionMatchPatterns: [WKWebExtension.MatchPattern : Date]

The currently granted permission match patterns and their expiration dates.

var grantedPermissions: [WKWebExtension.Permission : Date]

The currently granted permissions and their expiration dates.

var hasAccessToAllHosts: Bool

A Boolean value indicating if the currently granted permission match patterns set contains the `` pattern or any `*` host patterns.

var hasAccessToAllURLs: Bool

A Boolean value indicating if the currently granted permission match patterns set contains the `` pattern.

var hasAccessToPrivateData: Bool

A Boolean value indicating if the extension has access to private data.

var hasContentModificationRules: Bool

A boolean value indicating whether the extension includes rules used for content modification or blocking.

var hasInjectedContent: Bool

A Boolean value indicating whether the extension has script or stylesheet content that can be injected into webpages.

var hasRequestedOptionalAccessToAllHosts: Bool

A Boolean value indicating if the extension has requested optional access to all hosts.

var inspectionName: String?

The name shown when inspecting the background web view.

var isInspectable: Bool

Determines whether Web Inspector can inspect the WKWebView instances for this context.

var isLoaded: Bool

A Boolean value indicating if this context is loaded in an extension controller.

var openTabs: Set&lt;AnyHashable>

A set of open tabs in all open windows that are exposed to this extension.

var openWindows: [any WKWebExtensionWindow]

The open windows that are exposed to this extension.

var optionsPageURL: URL?

The URL of the extension’s options page, if the extension has one.

var overrideNewTabPageURL: URL?

The URL to use as an alternative to the default new tab page, if the extension has one.

var uniqueIdentifier: String

A unique identifier used to distinguish the extension from other extensions and target it for messages.

var unsupportedAPIs: Set&lt;String>!

Specifies unsupported APIs for this extension, making them `undefined` in JavaScript.

var webExtension: WKWebExtension

The extension this context represents.

var webExtensionController: WKWebExtensionController?

The extension controller this context is loaded in, otherwise `nil` if it isn’t loaded.

var webViewConfiguration: WKWebViewConfiguration?

The web view configuration to use for web views that load pages from this extension.

### Instance Methods

func action(for: (any WKWebExtensionTab)?) -> WKWebExtension.Action?

Retrieves the extension action for a given tab, or the default action if `nil` is passed.

func clearUserGesture(in: any WKWebExtensionTab)

Called by the app to clear a user gesture in a specific tab.

func command(for: NSEvent) -> WKWebExtension.Command?

Retrieves the command associated with the given event without performing it.

func didActivateTab(any WKWebExtensionTab, previousActiveTab: (any WKWebExtensionTab)?)

Called by the app when a tab is activated to notify only this specific extension.

func didChangeTabProperties(WKWebExtension.TabChangedProperties, for: any WKWebExtensionTab)

Called by the app when the properties of a tab are changed to fire appropriate events with only this extension.

func didCloseTab(any WKWebExtensionTab, windowIsClosing: Bool)

Called by the app when a tab is closed to fire appropriate events with only this extension.

func didCloseWindow(any WKWebExtensionWindow)

Called by the app when a window is closed to fire appropriate events with only this extension.

func didDeselectTabs([any WKWebExtensionTab])

Called by the app when tabs are deselected to fire appropriate events with only this extension.

func didFocusWindow((any WKWebExtensionWindow)?)

Called by the app when a window gains focus to fire appropriate events with only this extension.

func didMoveTab(any WKWebExtensionTab, from: Int, in: (any WKWebExtensionWindow)?)

Called by the app when a tab is moved to fire appropriate events with only this extension.

func didOpenTab(any WKWebExtensionTab)

Called by the app when a new tab is opened to fire appropriate events with only this extension.

func didOpenWindow(any WKWebExtensionWindow)

Called by the app when a new window is opened to fire appropriate events with only this extension.

func didReplaceTab(any WKWebExtensionTab, with: any WKWebExtensionTab)

Called by the app when a tab is replaced by another tab to fire appropriate events with only this extension.

func didSelectTabs([any WKWebExtensionTab])

Called by the app when tabs are selected to fire appropriate events with only this extension.

func hasAccess(to: URL) -> Bool

Checks the specified URL against the currently granted permission match patterns.

func hasAccess(to: URL, in: (any WKWebExtensionTab)?) -> Bool

Checks the specified URL against the currently granted permission match patterns in a specific tab.

func hasActiveUserGesture(in: any WKWebExtensionTab) -> Bool

Indicates if a user gesture is currently active in the specified tab.

func hasInjectedContent(for: URL) -> Bool

Checks if the extension has script or stylesheet content that can be injected into the specified URL.

func hasPermission(WKWebExtension.Permission) -> Bool

Checks the specified permission against the currently granted permissions.

func hasPermission(WKWebExtension.Permission, in: (any WKWebExtensionTab)?) -> Bool

Checks the specified permission against the currently granted permissions in a specific tab.

func loadBackgroundContent(completionHandler: ((any Error)?) -> Void)

Loads the background content if needed for the extension.

func menuItems(for: any WKWebExtensionTab) -> [UIMenuElement]

Retrieves the menu items for a given tab.

func performAction(for: (any WKWebExtensionTab)?)

Performs the extension action associated with the specified tab or performs the default action if `nil` is passed.

func performCommand(WKWebExtension.Command)

Performs the specified command, triggering events specific to this extension.

func performCommand(for: UIKeyCommand) -> Bool

Performs the command associated with the given key command.

func performCommand(for: NSEvent) -> Bool

Performs the command associated with the given event.

func permissionStatus(for: WKWebExtension.Permission) -> WKWebExtensionContext.PermissionStatus

Checks the specified permission against the currently denied, granted, and requested permissions.

func permissionStatus(for: WKWebExtension.MatchPattern) -> WKWebExtensionContext.PermissionStatus

Checks the specified match pattern against the currently denied, granted, and requested permission match patterns.

func permissionStatus(for: URL) -> WKWebExtensionContext.PermissionStatus

Checks the specified URL against the currently denied, granted, and requested permission match patterns.

func permissionStatus(for: WKWebExtension.Permission, in: (any WKWebExtensionTab)?) -> WKWebExtensionContext.PermissionStatus

Checks the specified permission against the currently denied, granted, and requested permissions.

func permissionStatus(for: URL, in: (any WKWebExtensionTab)?) -> WKWebExtensionContext.PermissionStatus

Checks the specified URL against the currently denied, granted, and requested permission match patterns.

func permissionStatus(for: WKWebExtension.MatchPattern, in: (any WKWebExtensionTab)?) -> WKWebExtensionContext.PermissionStatus

Checks the specified match pattern against the currently denied, granted, and requested permission match patterns.

func setPermissionStatus(WKWebExtensionContext.PermissionStatus, for: WKWebExtension.Permission)

Sets the status of a permission with a distant future expiration date.

func setPermissionStatus(WKWebExtensionContext.PermissionStatus, for: URL)

Sets the permission status of a URL with a distant future expiration date.

func setPermissionStatus(WKWebExtensionContext.PermissionStatus, for: WKWebExtension.MatchPattern)

Sets the status of a match pattern with a distant future expiration date.

func setPermissionStatus(WKWebExtensionContext.PermissionStatus, for: URL, expirationDate: Date?)

Sets the permission status of a URL with a distant future expiration date.

func setPermissionStatus(WKWebExtensionContext.PermissionStatus, for: WKWebExtension.Permission, expirationDate: Date?)

Sets the status of a permission with a specific expiration date.

func setPermissionStatus(WKWebExtensionContext.PermissionStatus, for: WKWebExtension.MatchPattern, expirationDate: Date?)

Sets the status of a match pattern with a specific expiration date.

func userGesturePerformed(in: any WKWebExtensionTab)

Should be called by the app when a user gesture is performed in a specific tab.

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

### Web extensions

class WKWebExtension

An object that encapsulates a web extension’s resources that the manifest file defines.

protocol WKWebExtensionTab

A protocol with methods that represent a tab to web extensions.

protocol WKWebExtensionWindow

A protocol with methods that represent a window to web extensions.

class WKWebExtensionController

An object that manages a set of loaded extension contexts.

protocol WKWebExtensionControllerDelegate

A group of methods you use to customize web extension interactions.

