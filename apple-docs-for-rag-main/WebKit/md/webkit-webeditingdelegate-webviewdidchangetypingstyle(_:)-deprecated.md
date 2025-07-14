

- WebKit
- WebEditingDelegate
-  webViewDidChangeTypingStyle(\_:) Deprecated

Instance Method

# webViewDidChangeTypingStyle(\_:)

Sent by the default notification center when the user changes the typing style in the web view.

macOS 10.3–10.14Deprecated

``` source
optional func webViewDidChangeTypingStyle(_ notification: Notification!)
```

## Parameters 

`notification`  

Always set to WebViewDidChangeTypingStyleNotification. You can retrieve the `WebView` object by sending `object` to `notification`.

## See Also

### Related Documentation

func webView(WebView!, shouldChangeTypingStyle: DOMCSSStyleDeclaration!, toStyle: DOMCSSStyleDeclaration!) -> Bool

Returns whether the user should be allowed to change the typing style in a web view.

Deprecated

