

- WebKit
- WebUIDelegate
-  webViewHeaderHeight(\_:) Deprecated

Instance Method

# webViewHeaderHeight(\_:)

Returns the height of the web view’s printed page header.

macOS 10.3–10.14Deprecated

``` source
optional func webViewHeaderHeight(_ sender: WebView!) -> Float
```

## Parameters 

`sender`  

The web view that sent the message.

## Return Value

The height of the web view’s printed page header. Returns `0.0` if no space is reserved for the header.

## Discussion

The height returned by this method is used to calculate the rectangle passed to the webView(_:drawHeaderIn:) method.

## See Also

### Printing

func webView(WebView!, print: WebFrameView!)

Prints the contents of a web frame view.

Deprecated

func webViewFooterHeight(WebView!) -> Float

Returns the height of the web view’s printed page footer.

Deprecated

func webView(WebView!, drawHeaderIn: NSRect)

Draws the web view’s header in the specified rectangle.

Deprecated

func webView(WebView!, drawFooterIn: NSRect)

Draws the web view’s footer in the specified rectangle.

Deprecated

