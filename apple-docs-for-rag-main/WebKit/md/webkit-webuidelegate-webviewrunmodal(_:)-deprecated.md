

- WebKit
- WebUIDelegate
-  webViewRunModal(\_:) Deprecated

Instance Method

# webViewRunModal(\_:)

Displays a web view in a modal window.

macOS 10.3–10.14Deprecated

``` source
optional func webViewRunModal(_ sender: WebView!)
```

## Parameters 

`sender`  

The web view that sent the message.

## Discussion

This method should display and order front a modal window containing the specified web view. This method is invoked after the webView(_:createWebViewModalDialogWith:) method is used to create a new window.

## See Also

### Creating and Closing Windows

func webView(WebView!, createWebViewModalDialogWith: URLRequest!) -> WebView!

Creates a modal window containing a web view that loads the specified request.

Deprecated

func webView(WebView!, createWebViewWith: URLRequest!) -> WebView!

Creates a window containing a web view to load the specified request.

Deprecated

func webViewClose(WebView!)

Closes a web view in a window.

Deprecated

