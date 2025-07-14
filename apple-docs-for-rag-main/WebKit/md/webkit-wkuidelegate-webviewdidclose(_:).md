

- WebKit
- WKUIDelegate
-  webViewDidClose(\_:) 

Instance Method

# webViewDidClose(\_:)

Notifies your app that the DOM window closed successfully.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
@MainActor
optional func webViewDidClose(_ webView: WKWebView)
```

## Parameters 

`webView`  

The web view invoking the delegate method.

## Discussion

Your app should remove the web view from the view hierarchy and update the UI as needed, for instance by closing the containing browser tab or window.

## See Also

### Creating and closing the web view

func webView(WKWebView, createWebViewWith: WKWebViewConfiguration, for: WKNavigationAction, windowFeatures: WKWindowFeatures) -> WKWebView?

Creates a new web view.

