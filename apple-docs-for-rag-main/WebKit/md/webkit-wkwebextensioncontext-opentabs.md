

- WebKit
- WKWebExtensionContext
-  openTabs 

Instance Property

# openTabs

A set of open tabs in all open windows that are exposed to this extension.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
var openTabs: Set { get }
```

## Discussion

Provides a set of tabs in all open windows that are visible to the extension, as updated by the didOpenTab(_:) and didCloseTab:windowIsClosing: methods.

Initially populated by the tabs in the windows returned by the extension controller delegate method webExtensionController(_:openWindowsFor:).

## See Also

### Related Documentation

func didOpenTab(any WKWebExtensionTab)

Called by the app when a new tab is opened to fire appropriate events with only this extension.

