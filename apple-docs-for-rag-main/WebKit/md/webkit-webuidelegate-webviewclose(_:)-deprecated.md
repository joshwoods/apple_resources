

- WebKit
- WebUIDelegate
-  webViewClose(\_:) Deprecated

Instance Method

# webViewClose(\_:)

Closes a web view in a window.

macOS 10.3–10.14Deprecated

``` source
optional func webViewClose(_ sender: WebView!)
```

## Parameters 

`sender`  

The web view that sent the message.

## Discussion

If you display multiple web views in a window then you might want to close only `sender` in your implementation. By default, this method sends the close() method to the NSWindow object that contains `sender`.

## See Also

### Creating and Closing Windows

func webView(WebView!, createWebViewModalDialogWith: URLRequest!) -> WebView!

Creates a modal window containing a web view that loads the specified request.

Deprecated

func webViewRunModal(WebView!)

Displays a web view in a modal window.

Deprecated

func webView(WebView!, createWebViewWith: URLRequest!) -> WebView!

Creates a window containing a web view to load the specified request.

Deprecated

