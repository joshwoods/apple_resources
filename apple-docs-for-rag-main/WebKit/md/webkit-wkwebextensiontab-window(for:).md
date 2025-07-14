

- WebKit
- WKWebExtensionTab
-  window(for:) 

Instance Method

# window(for:)

Called when the window containing the tab is needed.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
optional func window(for context: WKWebExtensionContext) -> (any WKWebExtensionWindow)?
```

## Parameters 

`context`  

The context in which the web extension is running.

## Discussion

Defaults to `nil` if not implemented.

