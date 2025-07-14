

- WebKit
- WebFrameLoadDelegate
-  webView(\_:didFailLoadWithError:for:) Deprecated

Instance Method

# webView(\_:didFailLoadWithError:for:)

Called when an error occurs loading a committed data source.

macOS 10.3–10.14Deprecated

``` source
optional func webView(
    _ sender: WebView!,
    didFailLoadWithError error: (any Error)!,
    for frame: WebFrame!
)
```

## Parameters 

`sender`  

The web view containing the frame.

`error`  

The type of error that occurred during the load.

`frame`  

The frame being loaded.

## Discussion

This method is called after the data source has been committed but resulted in an error.

