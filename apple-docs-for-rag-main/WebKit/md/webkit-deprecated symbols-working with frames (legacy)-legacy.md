

- WebKit
- Deprecated Symbols
-  Working with Frames (legacy) 

API Collection

# Working with Frames (legacy)

## Topics

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

protocol WebFrameLoadDelegateDeprecated

## See Also

### WebKit Legacy APIs

Document Object Models API (Legacy)

Setting Up a Web View (Legacy)

Accessing Previous Webpages (Legacy)

Archiving Webpages (Legacy)

Loading Resources (Legacy)

Downloading Information (Legacy)

Opening a File (Legacy)

Setting Policies (Legacy)

Implementing Plugins (Legacy)

Incorporating Scripts (Legacy)

Working With Document Web Views (Legacy)

