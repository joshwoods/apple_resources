

- WebKit
- WebUIDelegate
-  webViewIsResizable(\_:) Deprecated

Instance Method

# webViewIsResizable(\_:)

Returns a Boolean value indicating whether a web view’s window can be resized.

macOS 10.3–10.14Deprecated

``` source
optional func webViewIsResizable(_ sender: WebView!) -> Bool
```

## Parameters 

`sender`  

The web view that sent the message.

## Return Value

true if the web view’s window can be resized; otherwise, false.

## Discussion

If you display multiple web views in a window then your user interface delegate should implement this method to handle this special case.

## See Also

### Moving and Resizing Windows

func webView(WebView!, setResizable: Bool)

Sets whether a web view’s window can be resized.

Deprecated

func webView(WebView!, setFrame: NSRect)

Sets the frame rectangle of a web view’s window to the specified frame size.

Deprecated

func webViewFrame(WebView!) -> NSRect

Returns the frame rectangle of a web view’s window.

Deprecated

