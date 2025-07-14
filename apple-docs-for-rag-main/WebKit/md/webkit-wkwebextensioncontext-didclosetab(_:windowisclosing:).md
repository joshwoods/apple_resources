

- WebKit
- WKWebExtensionContext
-  didCloseTab(\_:windowIsClosing:) 

Instance Method

# didCloseTab(\_:windowIsClosing:)

Called by the app when a tab is closed to fire appropriate events with only this extension.

iOS 18.4+iPadOS 18.4+Mac CatalystmacOS 15.4+visionOS 2.4+

``` source
@MainActor @preconcurrency
func didCloseTab(
    _ closedTab: any WKWebExtensionTab,
    windowIsClosing: Bool = false
)
```

## Parameters 

`closedTab`  

The tab that was closed.

`windowIsClosing`  

A Boolean value indicating whether the window containing the tab is also closing.

## Discussion

This method informs only the specific extension of the closure of a tab. If the intention is to inform all loaded extensions consistently, you should use the respective method on the extension controller instead.

## See Also

### Related Documentation

func didOpenTab(any WKWebExtensionTab)

Called by the app when a new tab is opened to fire appropriate events with only this extension.

var openTabs: Set&lt;AnyHashable>

A set of open tabs in all open windows that are exposed to this extension.

