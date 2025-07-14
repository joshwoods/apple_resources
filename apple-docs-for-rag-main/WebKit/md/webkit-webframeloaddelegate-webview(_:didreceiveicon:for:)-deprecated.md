

- WebKit
- WebFrameLoadDelegate
-  webView(\_:didReceiveIcon:for:) Deprecated

Instance Method

# webView(\_:didReceiveIcon:for:)

Called when a page icon changes.

macOS 10.3–10.14Deprecated

``` source
optional func webView(
    _ sender: WebView!,
    didReceiveIcon image: NSImage!,
    for frame: WebFrame!
)
```

## Parameters 

`sender`  

The web view containing the frame.

`image`  

The page icon for a data source.

`frame`  

The frame being loaded.

## Discussion

This method may be invoked multiple times before all resources for `frame` are completely loaded. Sometimes a page uses a default icon or stored image that changes when the actual images is loaded.

