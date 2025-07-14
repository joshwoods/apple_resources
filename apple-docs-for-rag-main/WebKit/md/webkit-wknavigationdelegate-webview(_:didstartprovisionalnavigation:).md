

- WebKit
- WKNavigationDelegate
-  webView(\_:didStartProvisionalNavigation:) 

Instance Method

# webView(\_:didStartProvisionalNavigation:)

Tells the delegate that navigation from the main frame has started.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+

``` source
@MainActor
optional func webView(
    _ webView: WKWebView,
    didStartProvisionalNavigation navigation: WKNavigation!
)
```

## Parameters 

`webView`  

The web view that is loading the content.

`navigation`  

The navigation object associated with the load request.

## Mentioned in 

Replacing UIWebView in your app

## Discussion

The web view calls this method after it receives provisional approval to process a navigation request, but before it receives a response to that request.

## See Also

### Tracking the load progress of a request

func webView(WKWebView, didReceiveServerRedirectForProvisionalNavigation: WKNavigation!)

Tells the delegate that the web view received a server redirect for a request.

func webView(WKWebView, didCommit: WKNavigation!)

Tells the delegate that the web view has started to receive content for the main frame.

func webView(WKWebView, didFinish: WKNavigation!)

Tells the delegate that navigation is complete.

