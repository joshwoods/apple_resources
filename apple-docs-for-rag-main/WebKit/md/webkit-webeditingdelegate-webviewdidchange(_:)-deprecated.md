

- WebKit
- WebEditingDelegate
-  webViewDidChange(\_:) Deprecated

Instance Method

# webViewDidChange(\_:)

Sent by the default notification center when the user changes content in the web view.

macOS 10.3–10.14Deprecated

``` source
optional func webViewDidChange(_ notification: Notification!)
```

## Parameters 

`notification`  

Always set to WebViewDidChangeNotification. You can retrieve the `WebView` object by sending `object` to `notification`.

## See Also

### Related Documentation

func webView(WebView!, shouldInsert: DOMNode!, replacing: DOMRange!, given: WebViewInsertAction) -> Bool

Returns whether the user should be allowed to insert a node in place of a range of content.

Deprecated

func webView(WebView!, shouldInsertText: String!, replacing: DOMRange!, given: WebViewInsertAction) -> Bool

Returns whether a user should be allowed to insert text in place of a range of content.

Deprecated

func webView(WebView!, shouldDelete: DOMRange!) -> Bool

Returns whether the user should be allowed to delete a range of content.

Deprecated

