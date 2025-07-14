

- WebKit
- WebFrameLoadDelegate
-  webView(\_:willClose:) Deprecated

Instance Method

# webView(\_:willClose:)

Called when a frame will be closed.

macOS 10.3–10.14Deprecated

``` source
optional func webView(
    _ sender: WebView!,
    willClose frame: WebFrame!
)
```

## Parameters 

`sender`  

The web view containing the frame.

`frame`  

The frame being loaded.

## Discussion

Called right before WebKit is done with `frame` and the objects it owns.

## See Also

### Related Documentation

func webView(WebView!, willPerformClientRedirectTo: URL!, delay: TimeInterval, fire: Date!, for: WebFrame!)

Called when a frame receives a client redirect and before it is fired.

Deprecated

