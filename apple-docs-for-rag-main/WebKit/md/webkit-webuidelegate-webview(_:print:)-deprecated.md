

- WebKit
- WebUIDelegate
-  webView(\_:print:) Deprecated

Instance Method

# webView(\_:print:)

Prints the contents of a web frame view.

macOS 10.3–10.14Deprecated

``` source
optional func webView(
    _ sender: WebView!,
    print frameView: WebFrameView!
)
```

## Parameters 

`sender`  

The web view that sent the message.

`frameView`  

The web frame view whose contents to print.

## Discussion

This method is invoked when a script or a user wants to print a webpage. Typically, the delegate implements this method to prepare the web frame view content for printing. The web frame view can handle some content without intervention by the delegate. Send the documentViewShouldHandlePrint message to the web frame view to determine if it can handle printing. If this method returns true, then the delegate can print the content by sending the printDocumentView() message to the web frame view. Otherwise, the delegate can use printOperation(with:) to get an NSPrintOperation object to print the web frame view.

## See Also

### Printing

func webViewHeaderHeight(WebView!) -> Float

Returns the height of the web view’s printed page header.

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

