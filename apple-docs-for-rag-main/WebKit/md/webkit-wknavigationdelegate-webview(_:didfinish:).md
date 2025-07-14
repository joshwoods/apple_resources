

- WebKit
- WKNavigationDelegate
-  webView(\_:didFinish:) 

Instance Method

# webView(\_:didFinish:)

Tells the delegate that navigation is complete.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+

``` source
@MainActor
optional func webView(
    _ webView: WKWebView,
    didFinish navigation: WKNavigation!
)
```

## Parameters 

`webView`  

The web view that loaded the content.

`navigation`  

The navigation object that finished.

## Mentioned in 

Replacing UIWebView in your app

## See Also

### Tracking the load progress of a request

func webView(WKWebView, didStartProvisionalNavigation: WKNavigation!)

Tells the delegate that navigation from the main frame has started.

func webView(WKWebView, didReceiveServerRedirectForProvisionalNavigation: WKNavigation!)

Tells the delegate that the web view received a server redirect for a request.

func webView(WKWebView, didCommit: WKNavigation!)

Tells the delegate that the web view has started to receive content for the main frame.

