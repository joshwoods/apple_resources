

- WebKit
- WebUIDelegate
-  webView(\_:drawHeaderIn:) Deprecated

Instance Method

# webView(\_:drawHeaderIn:)

Draws the web view’s header in the specified rectangle.

macOS 10.3–10.14Deprecated

``` source
optional func webView(
    _ sender: WebView!,
    drawHeaderIn rect: NSRect
)
```

## Parameters 

`sender`  

The web view that sent the message.

`rect`  

The rectangle reserved for drawing the header.

## See Also

### Printing

func webView(WebView!, print: WebFrameView!)

Prints the contents of a web frame view.

Deprecated

func webViewHeaderHeight(WebView!) -> Float

Returns the height of the web view’s printed page header.

Deprecated

func webViewFooterHeight(WebView!) -> Float

Returns the height of the web view’s printed page footer.

Deprecated

func webView(WebView!, drawFooterIn: NSRect)

Draws the web view’s footer in the specified rectangle.

Deprecated

