

- WebKit
- WKWebExtensionController
-  didCloseTab(\_:windowIsClosing:) 

Instance Method

# didCloseTab(\_:windowIsClosing:)

Should be called by the app when a tab is closed to fire appropriate events with all loaded web extensions.

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

A boolean value indicating whether the window containing the tab is also closing.

## Discussion

This method informs all loaded extensions of the closing of a tab, ensuring consistent understanding across extensions.

If the intention is to inform only a specific extension, you should use the respective method on that extension’s context instead.

## See Also

### Related Documentation

func didOpenTab(any WKWebExtensionTab)

Should be called by the app when a new tab is opened to fire appropriate events with all loaded web extensions.

