

- WebKit
-  WKWebExtensionControllerDelegate 

Protocol

# WKWebExtensionControllerDelegate

A group of methods you use to customize web extension interactions.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
protocol WKWebExtensionControllerDelegate : NSObjectProtocol
```

## Topics

### Instance Methods

func webExtensionController(WKWebExtensionController, connectUsing: WKWebExtension.MessagePort, for: WKWebExtensionContext, completionHandler: ((any Error)?) -> Void)

Called when an extension context wants to establish a persistent connection to an application.

func webExtensionController(WKWebExtensionController, didUpdate: WKWebExtension.Action, forExtensionContext: WKWebExtensionContext)

Called when an action’s properties are updated.

func webExtensionController(WKWebExtensionController, focusedWindowFor: WKWebExtensionContext) -> (any WKWebExtensionWindow)?

Called when an extension context requests the currently focused window.

func webExtensionController(WKWebExtensionController, openNewTabUsing: WKWebExtension.TabConfiguration, for: WKWebExtensionContext, completionHandler: ((any WKWebExtensionTab)?, (any Error)?) -> Void)

Called when an extension context requests a new tab to be opened.

func webExtensionController(WKWebExtensionController, openNewWindowUsing: WKWebExtension.WindowConfiguration, for: WKWebExtensionContext, completionHandler: ((any WKWebExtensionWindow)?, (any Error)?) -> Void)

Called when an extension context requests a new window to be opened.

func webExtensionController(WKWebExtensionController, openOptionsPageFor: WKWebExtensionContext, completionHandler: ((any Error)?) -> Void)

Called when an extension context requests its options page to be opened.

func webExtensionController(WKWebExtensionController, openWindowsFor: WKWebExtensionContext) -> [any WKWebExtensionWindow]

Called when an extension context requests the list of ordered open windows.

func webExtensionController(WKWebExtensionController, presentActionPopup: WKWebExtension.Action, for: WKWebExtensionContext, completionHandler: ((any Error)?) -> Void)

Called when a popup is requested to be displayed for a specific action.

func webExtensionController(WKWebExtensionController, promptForPermissionMatchPatterns: Set&lt;WKWebExtension.MatchPattern>, in: (any WKWebExtensionTab)?, for: WKWebExtensionContext, completionHandler: (Set&lt;WKWebExtension.MatchPattern>, Date?) -> Void)

Called when an extension context requests access to a set of match patterns.

func webExtensionController(WKWebExtensionController, promptForPermissionToAccess: Set&lt;URL>, in: (any WKWebExtensionTab)?, for: WKWebExtensionContext, completionHandler: (Set&lt;URL>, Date?) -> Void)

Called when an extension context requests access to a set of URLs.

func webExtensionController(WKWebExtensionController, promptForPermissions: Set&lt;WKWebExtension.Permission>, in: (any WKWebExtensionTab)?, for: WKWebExtensionContext, completionHandler: (Set&lt;WKWebExtension.Permission>, Date?) -> Void)

Called when an extension context requests permissions.

func webExtensionController(WKWebExtensionController, sendMessage: Any, toApplicationWithIdentifier: String?, for: WKWebExtensionContext, replyHandler: (Any?, (any Error)?) -> Void)

Called when an extension context wants to send a one-time message to an application.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Web extensions

class WKWebExtension

An object that encapsulates a web extension’s resources that the manifest file defines.

protocol WKWebExtensionTab

A protocol with methods that represent a tab to web extensions.

protocol WKWebExtensionWindow

A protocol with methods that represent a window to web extensions.

class WKWebExtensionContext

An object that represents the runtime environment for a web extension.

class WKWebExtensionController

An object that manages a set of loaded extension contexts.

