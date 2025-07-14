

- WebKit
- WebFrameLoadDelegate
-  webView(\_:didStartProvisionalLoadFor:) Deprecated

Instance Method

# webView(\_:didStartProvisionalLoadFor:)

Called when a page load is in progress in a given frame.

macOS 10.3–10.14Deprecated

``` source
optional func webView(
    _ sender: WebView!,
    didStartProvisionalLoadFor frame: WebFrame!
)
```

## Parameters 

`sender`  

The web view containing the frame.

`frame`  

The frame being loaded.

## Discussion

This method is invoked when a new client request is made by `sender` to load a provisional data source for `frame`. This method may be invoked after sending load(_:) to a `WebFrame` object or as a consequence of the user clicking a link displayed in a web frame view. Delegates might implement this method to notify the user that a request is in progress. Additional information about the request can be obtained from the data source of `frame`.

## See Also

### Related Documentation

WebKit Objective-C Programming Guide

