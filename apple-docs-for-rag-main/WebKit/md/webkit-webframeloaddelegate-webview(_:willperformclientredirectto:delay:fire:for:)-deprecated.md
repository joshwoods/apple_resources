

- WebKit
- WebFrameLoadDelegate
-  webView(\_:willPerformClientRedirectTo:delay:fire:for:) Deprecated

Instance Method

# webView(\_:willPerformClientRedirectTo:delay:fire:for:)

Called when a frame receives a client redirect and before it is fired.

macOS 10.3–10.14Deprecated

``` source
optional func webView(
    _ sender: WebView!,
    willPerformClientRedirectTo URL: URL!,
    delay seconds: TimeInterval,
    fire date: Date!,
    for frame: WebFrame!
)
```

## Parameters 

`sender`  

The web view containing the frame.

`URL`  

The redirect location.

`seconds`  

The number of seconds from `date` before the redirect will be fired.

`date`  

The date and time to call the redirect.

`frame`  

The frame where the redirect occurred.

## Discussion

Delegates might implement this method to display progress while a client redirect is pending. If a client redirect is cancelled the webView(_:didCancelClientRedirectFor:) delegate method is invoked.

