

- WebKit
- WebUIDelegate
-  webViewFrame(\_:) Deprecated

Instance Method

# webViewFrame(\_:)

Returns the frame rectangle of a web view’s window.

macOS 10.3–10.14Deprecated

``` source
optional func webViewFrame(_ sender: WebView!) -> NSRect
```

## Parameters 

`sender`  

The web view that sent the message.

## Return Value

The frame rectangle of the web view’s window.

## See Also

### Moving and Resizing Windows

func webViewIsResizable(WebView!) -> Bool

Returns a Boolean value indicating whether a web view’s window can be resized.

Deprecated

func webView(WebView!, setResizable: Bool)

Sets whether a web view’s window can be resized.

Deprecated

func webView(WebView!, setFrame: NSRect)

Sets the frame rectangle of a web view’s window to the specified frame size.

Deprecated

