

- WebKit
- WKWebExtensionContext
-  didMoveTab(\_:from:in:) 

Instance Method

# didMoveTab(\_:from:in:)

Called by the app when a tab is moved to fire appropriate events with only this extension.

iOS 18.4+iPadOS 18.4+Mac CatalystmacOS 15.4+visionOS 2.4+

``` source
@MainActor @preconcurrency
func didMoveTab(
    _ movedTab: any WKWebExtensionTab,
    from index: Int,
    in oldWindow: (any WKWebExtensionWindow)? = nil
)
```

## Parameters 

`movedTab`  

The tab that was moved.

`index`  

The old index of the tab within the window.

`oldWindow`  

The window that the tab was moved from, or `nil` if the tab isn’t moving from an open window.

## Discussion

If the window is staying the same, the current window should be specified. This method informs only the specific extension that a tab has been moved. If the intention is to inform all loaded extensions consistently, you should use the respective method on the extension controller instead.

