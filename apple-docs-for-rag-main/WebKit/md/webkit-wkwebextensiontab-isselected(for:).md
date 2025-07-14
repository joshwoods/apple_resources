

- WebKit
- WKWebExtensionTab
-  isSelected(for:) 

Instance Method

# isSelected(for:)

Called when the selected state of the tab is needed.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
optional func isSelected(for context: WKWebExtensionContext) -> Bool
```

## Parameters 

`context`  

The context in which the web extension is running.

## Discussion

Defaults to `YES` for the active tab and `NO` for other tabs if not implemented.

