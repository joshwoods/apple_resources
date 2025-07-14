

- WebKit
- WebUIDelegate
-  webViewShow(\_:) Deprecated

Instance Method

# webViewShow(\_:)

Displays a web view’s window and moves it to the front.

macOS 10.3–10.14Deprecated

``` source
optional func webViewShow(_ sender: WebView!)
```

## Parameters 

`sender`  

The web view that sent the message.

## Discussion

This method is typically used after a call to webView(_:createWebViewWith:), which creates a new window. The new window is not ordered to the front (or even shown) unless you implement this method.

