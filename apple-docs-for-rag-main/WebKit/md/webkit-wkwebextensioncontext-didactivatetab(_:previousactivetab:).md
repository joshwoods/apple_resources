

- WebKit
- WKWebExtensionContext
-  didActivateTab(\_:previousActiveTab:) 

Instance Method

# didActivateTab(\_:previousActiveTab:)

Called by the app when a tab is activated to notify only this specific extension.

iOS 18.4+iPadOS 18.4+Mac CatalystmacOS 15.4+visionOS 2.4+

``` source
@MainActor @preconcurrency
func didActivateTab(
    _ activatedTab: any WKWebExtensionTab,
    previousActiveTab previousTab: (any WKWebExtensionTab)? = nil
)
```

## Parameters 

`activatedTab`  

The tab that has become active.

`previousTab`  

The tab that was active before. This parameter can be `nil` if there was no previously active tab.

## Discussion

This method informs only the specific extension of the tab activation. If the intention is to inform all loaded extensions consistently, you should use the respective method on the extension controller instead.

