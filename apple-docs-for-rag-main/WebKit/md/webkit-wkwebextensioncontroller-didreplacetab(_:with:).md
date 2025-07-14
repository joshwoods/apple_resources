

- WebKit
- WKWebExtensionController
-  didReplaceTab(\_:with:) 

Instance Method

# didReplaceTab(\_:with:)

Should be called by the app when a tab is replaced by another tab to fire appropriate events with all loaded web extensions.

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

This method informs all loaded extensions of the replacement of a tab, ensuring consistent understanding across extensions.

If the intention is to inform only a specific extension, you should use the respective method on that extension’s context instead.

