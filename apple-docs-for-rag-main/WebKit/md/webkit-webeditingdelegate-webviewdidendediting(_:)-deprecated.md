

- WebKit
- WebEditingDelegate
-  webViewDidEndEditing(\_:) Deprecated

Instance Method

# webViewDidEndEditing(\_:)

Sent by the default notification center when the user stops editing the web view.

macOS 10.3–10.14Deprecated

``` source
optional func webViewDidEndEditing(_ notification: Notification!)
```

## Parameters 

`notification`  

Always set to WebViewDidEndEditingNotification. You can retrieve the `WebView` object by sending `object` to `notification`.

## See Also

### Related Documentation

func webView(WebView!, shouldEndEditingIn: DOMRange!) -> Bool

Returns whether the user should be allowed to end editing.

Deprecated

func webViewDidBeginEditing(Notification!)

Sent by the default notification center when the user begins editing the web view.

Deprecated

