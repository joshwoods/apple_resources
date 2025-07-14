

- WebKit
- WebUIDelegate
-  webViewFocus(\_:) Deprecated

Instance Method

# webViewFocus(\_:)

Brings a web view’s window to the front and makes it the active window.

macOS 10.3–10.14Deprecated

``` source
optional func webViewFocus(_ sender: WebView!)
```

## Parameters 

`sender`  

The web view that sent the message.

## Discussion

By default, this method brings a web view’s window into focus. If you display multiple web views in a window then you might also want to focus the input on `sender`, using webView(_:makeFirstResponder:).

## See Also

### Making Windows Key and Main

func webViewUnfocus(WebView!)

Relinquishes focus on a web view’s window.

Deprecated

