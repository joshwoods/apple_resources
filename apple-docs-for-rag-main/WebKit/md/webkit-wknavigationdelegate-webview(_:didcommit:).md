

- WebKit
- WKNavigationDelegate
-  webView(\_:didCommit:) 

Instance Method

# webView(\_:didCommit:)

Tells the delegate that the web view has started to receive content for the main frame.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+

``` source
@MainActor
optional func webView(
    _ webView: WKWebView,
    didCommit navigation: WKNavigation!
)
```

## Parameters 

`webView`  

The web view that is loading the content.

`navigation`  

The navigation object that uniquely identifies the load request.

## Discussion

After the navigation delegate’s webView(_:decidePolicyFor:decisionHandler:) method approves the navigation response, the web view begins processing it. As changes become ready, the web view calls this method immediately before it starts to update the main frame.

## See Also

### Tracking the load progress of a request

func webView(WKWebView, didStartProvisionalNavigation: WKNavigation!)

Tells the delegate that navigation from the main frame has started.

func webView(WKWebView, didReceiveServerRedirectForProvisionalNavigation: WKNavigation!)

Tells the delegate that the web view received a server redirect for a request.

func webView(WKWebView, didFinish: WKNavigation!)

Tells the delegate that navigation is complete.

