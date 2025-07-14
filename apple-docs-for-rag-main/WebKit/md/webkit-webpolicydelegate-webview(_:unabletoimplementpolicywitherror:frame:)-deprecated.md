

- WebKit
- WebPolicyDelegate
-  webView(\_:unableToImplementPolicyWithError:frame:) Deprecated

Instance Method

# webView(\_:unableToImplementPolicyWithError:frame:)

Handles or drops events that were rejected by a policy maker.

macOS 10.3–10.14Deprecated

``` source
optional func webView(
    _ webView: WebView!,
    unableToImplementPolicyWithError error: (any Error)!,
    frame: WebFrame!
)
```

## Parameters 

`webView`  

The `WebView` object for which this object is the policy delegate.

`error`  

The error that occurred.

`frame`  

The frame in which the error occurred.

## Discussion

Delegates might implement this method to display or log an error message. If you do not implement this method, no action is taken.

