

- WebKit
- WKWebExtensionContext
-  openWindows 

Instance Property

# openWindows

The open windows that are exposed to this extension.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
var openWindows: [any WKWebExtensionWindow] { get }
```

## Discussion

Provides the windows that are open and visible to the extension, as updated by the didOpenWindow(_:) and didCloseWindow(_:) methods.

Initially populated by the windows returned by the extension controller delegate method webExtensionController(_:openWindowsFor:).

## See Also

### Related Documentation

func didOpenWindow(any WKWebExtensionWindow)

Called by the app when a new window is opened to fire appropriate events with only this extension.

func didCloseWindow(any WKWebExtensionWindow)

Called by the app when a window is closed to fire appropriate events with only this extension.

