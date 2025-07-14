

- WebKit
- WebUIDelegate
-  webView(\_:createWebViewWith:) Deprecated

Instance Method

# webView(\_:createWebViewWith:)

Creates a window containing a web view to load the specified request.

macOS 10.3–10.14Deprecated

``` source
optional func webView(
    _ sender: WebView!,
    createWebViewWith request: URLRequest!
) -> WebView!
```

## Parameters 

`sender`  

The web view that sent the message.

`request`  

The request to load.

## Return Value

The web view that is loading the request.

## Discussion

This method should begin loading the content for the specified request by sending load(_:) to its main frame. The new window should initially be hidden. Later, a webViewShow(_:) message is sent to the delegate of the new web view. By default, this method returns `nil`.

## See Also

### Creating and Closing Windows

func webView(WebView!, createWebViewModalDialogWith: URLRequest!) -> WebView!

Creates a modal window containing a web view that loads the specified request.

Deprecated

func webViewRunModal(WebView!)

Displays a web view in a modal window.

Deprecated

func webViewClose(WebView!)

Closes a web view in a window.

Deprecated

