

- WebKit
- WebFrameLoadDelegate
-  webView(\_:didFailProvisionalLoadWithError:for:) Deprecated

Instance Method

# webView(\_:didFailProvisionalLoadWithError:for:)

Called if an error occurs when starting to load data for a page.

macOS 10.3–10.14Deprecated

``` source
optional func webView(
    _ sender: WebView!,
    didFailProvisionalLoadWithError error: (any Error)!,
    for frame: WebFrame!
)
```

## Parameters 

`sender`  

The web view containing the frame.

`error`  

Specifies the type of error that occurred during the load.

`frame`  

The frame being loaded.

## Discussion

The frame continues to display the committed data source if there is one.

