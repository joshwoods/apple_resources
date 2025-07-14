

- WebKit
- WebFrameLoadDelegate
-  webView(\_:didCreateJavaScriptContext:for:) Deprecated

Instance Method

# webView(\_:didCreateJavaScriptContext:for:)

Notifies the delegate that a new JavaScript context has been created.

macOS 10.3–10.14Deprecated

``` source
optional func webView(
    _ webView: WebView!,
    didCreateJavaScriptContext context: JSContext!,
    for frame: WebFrame!
)
```

## Parameters 

`webView`  

The view sending the message.

`context`  

The JSContext representing the frame’s JavaScript window object.

`frame`  

The WebFrame to which the context belongs.

## Discussion

If a delegate implements this method along with either webView(_:didClearWindowObject:for:) or webView:windowScriptObjectAvailable:, only `webView:didCreateJavaScriptContext:forFrame:` will be invoked. This lets the delegate implement multiple versions to maintain backwards compatibility with older versions of WebKit.

