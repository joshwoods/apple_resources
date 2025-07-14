

- WebKit
- WKWebExtensionTab
-  size(for:) 

Instance Method

# size(for:)

Called when the size of the tab is needed.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
optional func size(for context: WKWebExtensionContext) -> CGSize
```

## Parameters 

`context`  

The context in which the web extension is running.

## Discussion

Defaults to size of the tab’s web view if not implemented.

