

- WebKit
- WebFrameLoadDelegate
-  webView(\_:didFinishLoadFor:) Deprecated

Instance Method

# webView(\_:didFinishLoadFor:)

Called when a page load completes.

macOS 10.3–10.14Deprecated

``` source
optional func webView(
    _ sender: WebView!,
    didFinishLoadFor frame: WebFrame!
)
```

## Parameters 

`sender`  

The web view containing the frame.

`frame`  

The frame being loaded.

## Discussion

This method is invoked when a location request for `frame` has completed; that is, when all the resources are done loading. Additional information about the request can be obtained from the data source of `frame`.

## See Also

### Related Documentation

func webView(WebView!, didStartProvisionalLoadFor: WebFrame!)

Called when a page load is in progress in a given frame.

Deprecated

