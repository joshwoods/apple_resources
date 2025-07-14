

- WebKit
- WebPolicyDelegate
-  webView(\_:decidePolicyForNewWindowAction:request:newFrameName:decisionListener:) Deprecated

Instance Method

# webView(\_:decidePolicyForNewWindowAction:request:newFrameName:decisionListener:)

Decides whether to allow a targeted navigation event, such as opening a link in a new window.

macOS 10.3–10.14Deprecated

``` source
optional func webView(
    _ webView: WebView!,
    decidePolicyForNewWindowAction actionInformation: [AnyHashable : Any]!,
    request: URLRequest!,
    newFrameName frameName: String!,
    decisionListener listener: (any WebPolicyDecisionListener)!
)
```

## Parameters 

`webView`  

The `WebView` object for which this object is the policy delegate.

`actionInformation`  

A description of the action that triggered the navigation request. The possible key-value pairs in this dictionary are defined in `Making content decisions`.

`request`  

The request for which the new window action is performed.

`frameName`  

The name of the new frame that contains the content returned from the request.

`listener`  

The `WebPolicyDecisionListener` object that receives the policy decision.

## Discussion

This method is invoked when a targeted navigation decision needs to be made. A targeted navigation typically opens a new window to display content. The receiver implements a policy decision by sending one of the WebPolicyDecisionListener protocol messages to `listener`. This method allows delegates to modify the behavior of targeted links which normally open a new window. Delegates might do something else, such as download or present the content in a special way. If this method sends use() to `listener` then the new window will be opened, and webView(_:decidePolicyForNavigationAction:request:frame:decisionListener:) will be invoked with a WebNavigationType.other as the value for the WebActionNavigationTypeKey key in the action dictionary.

The default behavior sends use() to `listener`.

