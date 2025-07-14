

- WebKit
- WebUIDelegate
-  webViewFirstResponder(\_:) Deprecated

Instance Method

# webViewFirstResponder(\_:)

Returns the first responder of the web view’s window.

macOS 10.3–10.14Deprecated

``` source
optional func webViewFirstResponder(_ sender: WebView!) -> NSResponder!
```

## Parameters 

`sender`  

The web view that sent the message.

## Return Value

The view or subview that currently has the input focus. It can return `nil` or the default first responder if the sender is not attached to a window or if another view (not in the window) has the focus.

## See Also

### Working with the Responder Chain

func webView(WebView!, makeFirstResponder: NSResponder!)

Sets the first responder of a web view’s window to the specified view.

Deprecated

