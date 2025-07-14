

- WebKit
- WKNavigationDelegate
-  webView(\_:shouldGoTo:willUseInstantBack:completionHandler:) 

Instance Method

# webView(\_:shouldGoTo:willUseInstantBack:completionHandler:)

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
optional func webView(
    _ webView: WKWebView,
    shouldGoTo backForwardListItem: WKBackForwardListItem,
    willUseInstantBack: Bool,
    completionHandler: @escaping (Bool) -> Void
)
```

``` source
@MainActor
optional func webView(
    _ webView: WKWebView,
    shouldGoTo backForwardListItem: WKBackForwardListItem,
    willUseInstantBack: Bool
) async -> Bool
```

