

- WebKit
- WKNavigationDelegate
-  webView(\_:decidePolicyFor:decisionHandler:) 

Instance Method

# webView(\_:decidePolicyFor:decisionHandler:)

Asks the delegate for permission to navigate to new content based on the specified action information.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+

``` source
@MainActor
optional func webView(
    _ webView: WKWebView,
    decidePolicyFor navigationAction: WKNavigationAction,
    decisionHandler: @escaping @MainActor (WKNavigationActionPolicy) -> Void
)
```

``` source
@MainActor
optional func webView(
    _ webView: WKWebView,
    decidePolicyFor navigationAction: WKNavigationAction
) async -> WKNavigationActionPolicy
```

## Parameters 

`webView`  

The web view from which the navigation request began.

`navigationAction`  

Details about the action that triggered the navigation request.

`decisionHandler`  

A completion handler block to call with the results about whether to allow or cancel the navigation. This handler has no return value and takes the following parameter:

policy  
A constant that indicates whether to cancel or allow the navigation. For a list of possible values, see WKNavigationActionPolicy.

## Mentioned in 

Replacing UIWebView in your app

## Discussion

Use this method to allow or deny a navigation request that originated with the specified action. The web view calls this method after the interaction occurs but before it attempts to load any content. If you implement this method, always execute the `decisionHandler` block at some point. You may execute it synchronously from your delegate method’s implementation, or execute it asynchronously after your method returns.

If your delegate object implements the webView(_:decidePolicyFor:preferences:decisionHandler:) method, the web view doesn’t call this method.

## See Also

### Allowing or denying navigation requests

func webView(WKWebView, decidePolicyFor: WKNavigationAction, preferences: WKWebpagePreferences, decisionHandler: (WKNavigationActionPolicy, WKWebpagePreferences) -> Void)

Asks the delegate for permission to navigate to new content based on the specified preferences and action information.

enum WKNavigationActionPolicy

Constants that indicate whether to allow or cancel navigation to a webpage from an action.

func webView(WKWebView, decidePolicyFor: WKNavigationResponse, decisionHandler: (WKNavigationResponsePolicy) -> Void)

Asks the delegate for permission to navigate to new content after the response to the navigation request is known.

enum WKNavigationResponsePolicy

Constants that indicate whether to allow or cancel navigation to a webpage from a response.

