

- WebKit
- WebUIDelegate
-  webView(\_:setResizable:) Deprecated

Instance Method

# webView(\_:setResizable:)

Sets whether a web view’s window can be resized.

macOS 10.3–10.14Deprecated

``` source
optional func webView(
    _ sender: WebView!,
    setResizable resizable: Bool
)
```

## Parameters 

`sender`  

The web view that sent the message.

`resizable`  

If true, the web view’s window can be resized; if false, the window is not resizable.

## Discussion

By default, this method sets the window containing a web view to be resizable. If you display multiple web views in a window then your user interface delegate should implement this method to handle this special case. If you do not implement this method, the `NSWindow` method showsResizeIndicator is sent to the window that contains `sender`.

## See Also

### Moving and Resizing Windows

func webViewIsResizable(WebView!) -> Bool

Returns a Boolean value indicating whether a web view’s window can be resized.

Deprecated

func webView(WebView!, setFrame: NSRect)

Sets the frame rectangle of a web view’s window to the specified frame size.

Deprecated

func webViewFrame(WebView!) -> NSRect

Returns the frame rectangle of a web view’s window.

Deprecated

