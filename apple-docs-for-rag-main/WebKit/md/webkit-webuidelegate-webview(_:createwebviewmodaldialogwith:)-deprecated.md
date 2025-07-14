

- WebKit
- WebUIDelegate
-  webView(\_:createWebViewModalDialogWith:) Deprecated

Instance Method

# webView(\_:createWebViewModalDialogWith:)

Creates a modal window containing a web view that loads the specified request.

macOS 10.3–10.14Deprecated

``` source
optional func webView(
    _ sender: WebView!,
    createWebViewModalDialogWith request: URLRequest!
) -> WebView!
```

## Parameters 

`sender`  

The web view that sent the message.

`request`  

The request to load.

## Return Value

The web view that is loading the specified request.

## Discussion

This method is invoked when JavaScript calls `window.showModalDialog`. It should create a new modal window containing the web view and initially hide the window. The webViewRunModal(_:) message is sent to the delegate to display the web view.

## See Also

### Related Documentation

WebKit Objective-C Programming Guide

### Creating and Closing Windows

func webViewRunModal(WebView!)

Displays a web view in a modal window.

Deprecated

func webView(WebView!, createWebViewWith: URLRequest!) -> WebView!

Creates a window containing a web view to load the specified request.

Deprecated

func webViewClose(WebView!)

Closes a web view in a window.

Deprecated

