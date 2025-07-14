

- WebKit
- WebPolicyDelegate
-  webView(\_:decidePolicyForNavigationAction:request:frame:decisionListener:) Deprecated

Instance Method

# webView(\_:decidePolicyForNavigationAction:request:frame:decisionListener:)

Routes a navigation action internally or to an external viewer.

macOS 10.3–10.14Deprecated

``` source
optional func webView(
    _ webView: WebView!,
    decidePolicyForNavigationAction actionInformation: [AnyHashable : Any]!,
    request: URLRequest!,
    frame: WebFrame!,
    decisionListener listener: (any WebPolicyDecisionListener)!
)
```

## Parameters 

`webView`  

The `WebView` object for which this object is the policy delegate.

`actionInformation`  

A description of the action that triggered the navigation request. The possible key-value pairs in this dictionary are defined in `Action Dictionary Keys`.

`request`  

The request for which the navigation is made.

`frame`  

The `WebFrame` object in which the action occurred.

`listener`  

The `WebPolicyDecisionListener` object that receives the policy decision.

## Discussion

This method is invoked when a navigation decision needs to be made. The web view implements a policy decision by sending one of the WebPolicyDecisionListener protocol messages to `listener`. This method is invoked whenever a server redirect is encountered, and before loading starts.

If you do not implement this method, the default behavior is used. The listener handles the navigation internally if the request is for an error page or if the canHandle(_:) method of the `NSURLConnection` class returns true when passed `request`. Otherwise, the listener ignores the navigation, and it is handled externally.

