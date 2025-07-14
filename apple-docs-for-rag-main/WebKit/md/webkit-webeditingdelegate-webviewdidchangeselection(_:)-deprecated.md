

- WebKit
- WebEditingDelegate
-  webViewDidChangeSelection(\_:) Deprecated

Instance Method

# webViewDidChangeSelection(\_:)

Sent by the default notification center when the user changes the selection in the web view.

macOS 10.3–10.14Deprecated

``` source
optional func webViewDidChangeSelection(_ notification: Notification!)
```

## Parameters 

`notification`  

Always set to WebViewDidChangeSelectionNotification. You can retrieve the `WebView` object by sending `object` to `notification`.

## See Also

### Related Documentation

func webView(WebView!, shouldChangeSelectedDOMRange: DOMRange!, to: DOMRange!, affinity: NSSelectionAffinity, stillSelecting: Bool) -> Bool

Returns whether the user should be allowed to change the selected range.

Deprecated

