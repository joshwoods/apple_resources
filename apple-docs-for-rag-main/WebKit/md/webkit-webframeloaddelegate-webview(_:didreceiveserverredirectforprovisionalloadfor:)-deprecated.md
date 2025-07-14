

- WebKit
- WebFrameLoadDelegate
-  webView(\_:didReceiveServerRedirectForProvisionalLoadFor:) Deprecated

Instance Method

# webView(\_:didReceiveServerRedirectForProvisionalLoadFor:)

Called when a provisional data source for a frame receives a server redirect.

macOS 10.3–10.14Deprecated

``` source
optional func webView(
    _ sender: WebView!,
    didReceiveServerRedirectForProvisionalLoadFor frame: WebFrame!
)
```

## Parameters 

`sender`  

The web view containing the frame.

`frame`  

The frame being loaded.

## Discussion

A *server redirect* is when one URL location is redirected to another. Additional information about the new request can be obtained from the data source of `frame`.

