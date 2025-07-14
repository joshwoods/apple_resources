

- WebKit
- WebUIDelegate
-  webViewUnfocus(\_:) Deprecated

Instance Method

# webViewUnfocus(\_:)

Relinquishes focus on a web view’s window.

macOS 10.3–10.14Deprecated

``` source
optional func webViewUnfocus(_ sender: WebView!)
```

## Parameters 

`sender`  

The web view that sent the message.

## Discussion

This method releases focus for the entire window. If you display multiple web views in a window, you might instead want to change the input focus to another view, using the webView(_:makeFirstResponder:) method.

## See Also

### Making Windows Key and Main

func webViewFocus(WebView!)

Brings a web view’s window to the front and makes it the active window.

Deprecated

