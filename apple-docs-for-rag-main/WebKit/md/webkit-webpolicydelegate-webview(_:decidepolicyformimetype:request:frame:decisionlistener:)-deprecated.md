

- WebKit
- WebPolicyDelegate
-  webView(\_:decidePolicyForMIMEType:request:frame:decisionListener:) Deprecated

Instance Method

# webView(\_:decidePolicyForMIMEType:request:frame:decisionListener:)

Decides whether to display content with a given MIME type.

macOS 10.3–10.14Deprecated

``` source
optional func webView(
    _ webView: WebView!,
    decidePolicyForMIMEType type: String!,
    request: URLRequest!,
    frame: WebFrame!,
    decisionListener listener: (any WebPolicyDecisionListener)!
)
```

## Parameters 

`webView`  

The associated web view.

`type`  

The MIME type of the content.

`request`  

The request to load the content.

`frame`  

The frame for displaying the content.

`listener`  

The object that receives the policy decision.

## Discussion

This method is invoked during the process of loading content for `request` after the `webView:didStartProvisionalLoadForFrame:` method in the `WebFrameLoadDelegate` protocol is called by the `WebView` object. The web view implements a policy decision by sending one of the WebPolicyDecisionListener protocol messages to `listener`.

If you do not implement this method, the default behavior is used. The listener is told to ignore the MIME type unless `webView` specifies it can handle the type in its canShowMIMEType(_:) method.

In some rare cases, multiple responses may be received for a single resource. This happens in the case of multipart/x-mixed-replace, also known as a “server push.” In this case, this method will be invoked multiple times.

