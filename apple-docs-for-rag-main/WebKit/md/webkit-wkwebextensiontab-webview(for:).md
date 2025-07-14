

- WebKit
- WKWebExtensionTab
-  webView(for:) 

Instance Method

# webView(for:)

Called when the web view for the tab is needed.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
optional func webView(for context: WKWebExtensionContext) -> WKWebView?
```

## Parameters 

`context`  

The context in which the web extension is running.

## Discussion

The web view’s WKWebViewConfiguration must have its webExtensionController property set to match the controller of the given context; otherwise `nil` will be used. Defaults to `nil` if not implemented. If `nil`, some critical features will not be available for this tab, such as content injection or modification.

