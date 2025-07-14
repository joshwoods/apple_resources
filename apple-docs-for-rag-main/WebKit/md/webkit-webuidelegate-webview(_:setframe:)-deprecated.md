

- WebKit
- WebUIDelegate
-  webView(\_:setFrame:) Deprecated

Instance Method

# webView(\_:setFrame:)

Sets the frame rectangle of a web view’s window to the specified frame size.

macOS 10.3–10.14Deprecated

``` source
optional func webView(
    _ sender: WebView!,
    setFrame frame: NSRect
)
```

## Parameters 

`sender`  

The web view that sent the message.

`frame`  

The frame size.

## Discussion

The sender invokes this method instead of setting the window’s frame directly, allowing delegates to augment the behavior by, for example, saving the original window size before resizing as a result of JavaScript running. If you do not implement this method, the `NSWindow` method setFrame(_:display:) is sent to the window that contains `sender`, with true passed as the display argument.

## See Also

### Moving and Resizing Windows

func webViewIsResizable(WebView!) -> Bool

Returns a Boolean value indicating whether a web view’s window can be resized.

Deprecated

func webView(WebView!, setResizable: Bool)

Sets whether a web view’s window can be resized.

Deprecated

func webViewFrame(WebView!) -> NSRect

Returns the frame rectangle of a web view’s window.

Deprecated

