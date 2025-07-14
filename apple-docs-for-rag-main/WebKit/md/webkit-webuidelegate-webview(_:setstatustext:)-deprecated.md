

- WebKit
- WebUIDelegate
-  webView(\_:setStatusText:) Deprecated

Instance Method

# webView(\_:setStatusText:)

Sets the status message displayed by a web view’s window, if any, to the specified text.

macOS 10.3–10.14Deprecated

``` source
optional func webView(
    _ sender: WebView!,
    setStatusText text: String!
)
```

## Parameters 

`sender`  

The web view that sent the message.

`text`  

The status message to display.

## Discussion

The delegate receives this message when a JavaScript function in the web view explicitly sets the status text. No action is taken if you do not implement this method.

## See Also

### Displaying Status Messages

func webViewStatusText(WebView!) -> String!

Returns the current status message from a web view’s window.

Deprecated

