

- WebKit
- WKWebExtensionContext
-  didReplaceTab(\_:with:) 

Instance Method

# didReplaceTab(\_:with:)

Called by the app when a tab is replaced by another tab to fire appropriate events with only this extension.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
func didReplaceTab(
    _ oldTab: any WKWebExtensionTab,
    with newTab: any WKWebExtensionTab
)
```

## Parameters 

`oldTab`  

The tab that was replaced.

`newTab`  

The tab that replaced the old tab.

## Discussion

This method informs only the specific extension that a tab has been replaced. If the intention is to inform all loaded extensions consistently, you should use the respective method on the extension controller instead.

