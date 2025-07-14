

- WebKit
-  WebFrameLoadDelegate Deprecated

Protocol

# WebFrameLoadDelegate

macOS 10.3–10.14Deprecated

``` source
protocol WebFrameLoadDelegate : NSObjectProtocol
```

## Topics

### Instance Methods

func webView(WebView!, didCancelClientRedirectFor: WebFrame!)

Called when a client redirect is cancelled.

func webView(WebView!, didChangeLocationWithinPageFor: WebFrame!)

Called when the scroll position within a frame changes.

func webView(WebView!, didClearWindowObject: WebScriptObject!, for: WebFrame!)

Called when the JavaScript window object in a frame is ready for loading.

func webView(WebView!, didCommitLoadFor: WebFrame!)

Called when content starts arriving for a page load.

func webView(WebView!, didCreateJavaScriptContext: JSContext!, for: WebFrame!)

Notifies the delegate that a new JavaScript context has been created.

func webView(WebView!, didFailLoadWithError: (any Error)!, for: WebFrame!)

Called when an error occurs loading a committed data source.

func webView(WebView!, didFailProvisionalLoadWithError: (any Error)!, for: WebFrame!)

Called if an error occurs when starting to load data for a page.

func webView(WebView!, didFinishLoadFor: WebFrame!)

Called when a page load completes.

func webView(WebView!, didReceiveIcon: NSImage!, for: WebFrame!)

Called when a page icon changes.

func webView(WebView!, didReceiveServerRedirectForProvisionalLoadFor: WebFrame!)

Called when a provisional data source for a frame receives a server redirect.

func webView(WebView!, didReceiveTitle: String!, for: WebFrame!)

Called when the page title of a frame loads or changes.

func webView(WebView!, didStartProvisionalLoadFor: WebFrame!)

Called when a page load is in progress in a given frame.

func webView(WebView!, willClose: WebFrame!)

Called when a frame will be closed.

func webView(WebView!, willPerformClientRedirectTo: URL!, delay: TimeInterval, fire: Date!, for: WebFrame!)

Called when a frame receives a client redirect and before it is fired.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Working with Frames (Legacy)

class WebFrame

A `WebFrame` object encapsulates the data displayed in a `WebFrameView` object. There is one `WebFrame` object per frame displayed in a `WebView`. An entire webpage is represented by a hierarchy of `WebFrame` objects in which the root object is called the **main frame**.

Deprecated

class WebDataSource

`WebDataSource` encapsulates the web content to be displayed in a web frame view. A `WebDataSource` object has a representation object, conforming to the `WebDocumentRepresentation` protocol, that holds the data in an appropriate format depending on the MIME type. You can extend WebKit to support new MIME types by implementing your own view and representation classes, and specifying the mapping between them using the registerClass(_:representationClass:forMIMEType:) `WebView` class method.

Deprecated

class WebFrameView

`WebFrameView` objects and their subviews display the web content contained in a frame. You never create instances of `WebFrameView` directly—`WebView` objects create and manage a hierarchy of `WebFrameView` objects, one for each frame. `WebFrameView` objects use a scroll view whose document view conforms to the WebDocumentView protocol.

Deprecated

