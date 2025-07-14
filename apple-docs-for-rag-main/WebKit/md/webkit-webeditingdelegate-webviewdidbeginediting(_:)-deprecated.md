

- WebKit
- WebEditingDelegate
-  webViewDidBeginEditing(\_:) Deprecated

Instance Method

# webViewDidBeginEditing(\_:)

Sent by the default notification center when the user begins editing the web view.

macOS 10.3–10.14Deprecated

``` source
optional func webViewDidBeginEditing(_ notification: Notification!)
```

## Parameters 

`notification`  

Always set to WebViewDidBeginEditingNotification. You can retrieve the `WebView` object by sending `object` to `notification`.

## See Also

### Related Documentation

func webView(WebView!, shouldBeginEditingIn: DOMRange!) -> Bool

Returns whether the user is allowed to edit a range of content in a web view.

Deprecated

func webViewDidEndEditing(Notification!)

Sent by the default notification center when the user stops editing the web view.

Deprecated

