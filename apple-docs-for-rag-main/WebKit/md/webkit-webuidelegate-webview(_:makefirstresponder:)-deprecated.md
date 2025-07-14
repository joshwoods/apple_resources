

- WebKit
- WebUIDelegate
-  webView(\_:makeFirstResponder:) Deprecated

Instance Method

# webView(\_:makeFirstResponder:)

Sets the first responder of a web view’s window to the specified view.

macOS 10.3–10.14Deprecated

``` source
optional func webView(
    _ sender: WebView!,
    makeFirstResponder responder: NSResponder!
)
```

## Parameters 

`sender`  

The web view that sent the message.

`responder`  

A view in the web view’s hierarchy.

## Discussion

You can ignore this message if `sender` is not yet attached to a window.

## See Also

### Working with the Responder Chain

func webViewFirstResponder(WebView!) -> NSResponder!

Returns the first responder of the web view’s window.

Deprecated

