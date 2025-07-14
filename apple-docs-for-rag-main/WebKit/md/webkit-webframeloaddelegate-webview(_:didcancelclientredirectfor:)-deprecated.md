

- WebKit
- WebFrameLoadDelegate
-  webView(\_:didCancelClientRedirectFor:) Deprecated

Instance Method

# webView(\_:didCancelClientRedirectFor:)

Called when a client redirect is cancelled.

macOS 10.3–10.14Deprecated

``` source
optional func webView(
    _ sender: WebView!,
    didCancelClientRedirectFor frame: WebFrame!
)
```

## Parameters 

`sender`  

The web view containing the frame.

`frame`  

The frame being loaded.

## Discussion

This might happen if a frame changes locations before a pending client redirect is fired. The client redirect occurred in `frame`.

