

- WebKit
-  WKWebExtensionController 

Class

# WKWebExtensionController

An object that manages a set of loaded extension contexts.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
class WKWebExtensionController
```

## Overview

You can have one or more extension controller instances, allowing different parts of the app to use different sets of extensions.

You can associate a controller with WKWebView using the webExtensionController property on WKWebViewConfiguration.

## Topics

### Initializers

init()

Returns a web extension controller initialized with the default configuration.

init(configuration: WKWebExtensionController.Configuration)

Returns a web extension controller initialized with the specified configuration.

### Instance Properties

var configuration: WKWebExtensionController.Configuration

A copy of the configuration with which the web extension controller was initialized.

var delegate: (any WKWebExtensionControllerDelegate)?

The extension controller delegate.

var extensionContexts: Set&lt;WKWebExtensionContext>

A set of all the currently loaded extension contexts.

var extensions: Set&lt;WKWebExtension>

A set of all the currently loaded extensions.

### Instance Methods

func didActivateTab(any WKWebExtensionTab, previousActiveTab: (any WKWebExtensionTab)?)

Should be called by the app when a tab is activated to notify all loaded web extensions.

func didChangeTabProperties(WKWebExtension.TabChangedProperties, for: any WKWebExtensionTab)

Should be called by the app when the properties of a tab are changed to fire appropriate events with all loaded web extensions.

func didCloseTab(any WKWebExtensionTab, windowIsClosing: Bool)

Should be called by the app when a tab is closed to fire appropriate events with all loaded web extensions.

func didCloseWindow(any WKWebExtensionWindow)

Should be called by the app when a window is closed to fire appropriate events with all loaded web extensions.

func didDeselectTabs([any WKWebExtensionTab])

Should be called by the app when tabs are deselected to fire appropriate events with all loaded web extensions.

func didFocusWindow((any WKWebExtensionWindow)?)

Should be called by the app when a window gains focus to fire appropriate events with all loaded web extensions.

func didMoveTab(any WKWebExtensionTab, from: Int, in: (any WKWebExtensionWindow)?)

Should be called by the app when a tab is moved to fire appropriate events with all loaded web extensions.

func didOpenTab(any WKWebExtensionTab)

Should be called by the app when a new tab is opened to fire appropriate events with all loaded web extensions.

func didOpenWindow(any WKWebExtensionWindow)

Should be called by the app when a new window is opened to fire appropriate events with all loaded web extensions.

func didReplaceTab(any WKWebExtensionTab, with: any WKWebExtensionTab)

Should be called by the app when a tab is replaced by another tab to fire appropriate events with all loaded web extensions.

func didSelectTabs([any WKWebExtensionTab])

Should be called by the app when tabs are selected to fire appropriate events with all loaded web extensions.

func extensionContext(for: URL) -> WKWebExtensionContext?

Returns a loaded extension context matching the specified URL.

func extensionContext(for: WKWebExtension) -> WKWebExtensionContext?

Returns a loaded extension context for the specified extension.

func fetchDataRecord(ofTypes: Set&lt;WKWebExtension.DataType>, for: WKWebExtensionContext, completionHandler: (WKWebExtension.DataRecord?) -> Void)

Fetches a data record containing the given extension data types for a specific known web extension context.

func fetchDataRecords(ofTypes: Set&lt;WKWebExtension.DataType>, completionHandler: ([WKWebExtension.DataRecord]) -> Void)

Fetches data records containing the given extension data types for all known extensions.

func load(WKWebExtensionContext) throws

Loads the specified extension context.

func removeData(ofTypes: Set&lt;WKWebExtension.DataType>, from: [WKWebExtension.DataRecord], completionHandler: () -> Void)

Removes extension data of the given types for the given data records.

func unload(WKWebExtensionContext) throws

Unloads the specified extension context.

### Type Properties

class var allExtensionDataTypes: Set&lt;WKWebExtension.DataType>

Returns a set of all available extension data types.

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

class WKWebExtensionContext

An object that represents the runtime environment for a web extension.

protocol WKWebExtensionControllerDelegate

A group of methods you use to customize web extension interactions.

