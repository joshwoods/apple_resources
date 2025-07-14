

- WebKit
- WebUIDelegate
-  webViewStatusText(\_:) Deprecated

Instance Method

# webViewStatusText(\_:)

Returns the current status message from a web view’s window.

macOS 10.3–10.14Deprecated

``` source
optional func webViewStatusText(_ sender: WebView!) -> String!
```

## Parameters 

`sender`  

The web view that sent the message.

## Return Value

The status message displayed in the web view’s window if one has been set with the webView(_:setStatusText:) method; otherwise, `nil`.

## See Also

### Displaying Status Messages

func webView(WebView!, setStatusText: String!)

Sets the status message displayed by a web view’s window, if any, to the specified text.

Deprecated

