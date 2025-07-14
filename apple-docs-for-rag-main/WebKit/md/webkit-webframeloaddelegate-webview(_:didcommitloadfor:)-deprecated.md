

- WebKit
- WebFrameLoadDelegate
-  webView(\_:didCommitLoadFor:) Deprecated

Instance Method

# webView(\_:didCommitLoadFor:)

Called when content starts arriving for a page load.

macOS 10.3–10.14Deprecated

``` source
optional func webView(
    _ sender: WebView!,
    didCommitLoadFor frame: WebFrame!
)
```

## Parameters 

`sender`  

The web view containing the frame.

`frame`  

The frame being loaded.

## Discussion

This method is invoked when a data source transitions from a provisional to committed state—that is, once the data source of `frame` has received one byte or more of data. This method is invoked after a webView(_:didStartProvisionalLoadFor:) message but before a `webView:didFinishLoadForFrame:` message is sent to the delegate.

In some cases, a single frame load may be committed more than once. This happens in the case of multipart/x-mixed-replace, also known as a “server push.” In this case, a single frame load results in multiple documents loaded in sequence. This method is invoked once for each document that is successfully loaded.

