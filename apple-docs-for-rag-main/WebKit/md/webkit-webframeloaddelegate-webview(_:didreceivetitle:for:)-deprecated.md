

- WebKit
- WebFrameLoadDelegate
-  webView(\_:didReceiveTitle:for:) Deprecated

Instance Method

# webView(\_:didReceiveTitle:for:)

Called when the page title of a frame loads or changes.

macOS 10.3–10.14Deprecated

``` source
optional func webView(
    _ sender: WebView!,
    didReceiveTitle title: String!,
    for frame: WebFrame!
)
```

## Parameters 

`sender`  

The web view containing the frame.

`title`  

The newly loaded title.

`frame`  

The frame being loaded.

## Discussion

This method may be invoked multiple times before all resources for `frame` are completely loaded. Delegates can implement this message to display the page title to the user.

