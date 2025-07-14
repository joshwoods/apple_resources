

- WebKit
- WebFrameLoadDelegate
-  webView(\_:didChangeLocationWithinPageFor:) Deprecated

Instance Method

# webView(\_:didChangeLocationWithinPageFor:)

Called when the scroll position within a frame changes.

macOS 10.3–10.14Deprecated

``` source
optional func webView(
    _ sender: WebView!,
    didChangeLocationWithinPageFor frame: WebFrame!
)
```

## Parameters 

`sender`  

The web view containing the frame.

`frame`  

The frame being loaded.

## Discussion

Typically invoked when the user clicks on an anchor within a page. Additional information about the request can be obtained from the data source of `frame`.

