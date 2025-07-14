

- WebKit
-  WKWebExtensionWindow 

Protocol

# WKWebExtensionWindow

A protocol with methods that represent a window to web extensions.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
protocol WKWebExtensionWindow : NSObjectProtocol
```

## Topics

### Instance Methods

func activeTab(for: WKWebExtensionContext) -> (any WKWebExtensionTab)?

Called when the active tab is needed for the window.

func close(for: WKWebExtensionContext, completionHandler: ((any Error)?) -> Void)

Called to close the window.

func focus(for: WKWebExtensionContext, completionHandler: ((any Error)?) -> Void)

Called to focus the window.

func frame(for: WKWebExtensionContext) -> CGRect

Called when the frame of the window is needed.

func isPrivate(for: WKWebExtensionContext) -> Bool

Called when the private state of the window is needed.

func screenFrame(for: WKWebExtensionContext) -> CGRect

Called when the screen frame containing the window is needed.

func setFrame(CGRect, for: WKWebExtensionContext, completionHandler: ((any Error)?) -> Void)

Called to set the frame of the window.

func setWindowState(WKWebExtension.WindowState, for: WKWebExtensionContext, completionHandler: ((any Error)?) -> Void)

Called to set the state of the window.

func tabs(for: WKWebExtensionContext) -> [any WKWebExtensionTab]

Called when the tabs are needed for the window.

func windowState(for: WKWebExtensionContext) -> WKWebExtension.WindowState

Called when the state of the window is needed.

func windowType(for: WKWebExtensionContext) -> WKWebExtension.WindowType

Called when the type of the window is needed.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Web extensions

class WKWebExtension

An object that encapsulates a web extension’s resources that the manifest file defines.

protocol WKWebExtensionTab

A protocol with methods that represent a tab to web extensions.

class WKWebExtensionContext

An object that represents the runtime environment for a web extension.

class WKWebExtensionController

An object that manages a set of loaded extension contexts.

protocol WKWebExtensionControllerDelegate

A group of methods you use to customize web extension interactions.

