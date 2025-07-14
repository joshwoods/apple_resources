

- WebKit
-  WebDataSource Deprecated

Class

# WebDataSource

`WebDataSource` encapsulates the web content to be displayed in a web frame view. A `WebDataSource` object has a representation object, conforming to the `WebDocumentRepresentation` protocol, that holds the data in an appropriate format depending on the MIME type. You can extend WebKit to support new MIME types by implementing your own view and representation classes, and specifying the mapping between them using the registerClass(_:representationClass:forMIMEType:) `WebView` class method.

macOS 10.3–10.14Deprecated

``` source
class WebDataSource
```

## Overview

`WebDataSource` objects have an associated initial request, possibly a modified request, and a response object. Since the data source may be in the process of being loaded, you should check the state of a data source using isLoading before accessing its data. Use data to get the raw data. Use the representation method to get the actual representation object and query it for more details.

## Topics

### Initializing an instance

init!(request: URLRequest!)

initializes a data source with a URL request.

### Querying page data and state

var data: Data!

The raw data that represents the data source’s content.

var isLoading: Bool

A Boolean that indicates whether the data source is loading its content.

var pageTitle: String!

The title of the data source’s page.

var representation: (any WebDocumentRepresentation)!

The data source’s representation depending on its MIME type.

var textEncodingName: String!

The text encoding for the data source’s web view, if set, or the text encoding of the response.

### Getting the request and response

var initialRequest: URLRequest!

A reference to the original request that was used to load the web content.

var request: NSMutableURLRequest!

The request that was used to create the data source.

var response: URLResponse!

The response for this data source.

### Getting the web frame

var webFrame: WebFrame!

The web frame that represents this data source.

### Getting an unreachable URL

var unreachableURL: URL!

The data source’s unreachable URL.

### Getting a web archive

var webArchive: WebArchive!

A web archive representing the data source, its subresources, and subframes.

### Accessing subresources

var mainResource: WebResource!

A`WebResource` object representing the data source.

func addSubresource(WebResource!)

Adds a resource to the data source’s list of subresources.

func subresource(for: URL!) -> WebResource!

Returns a subresource for the given URL.

var subresources: [Any]!

The data source’s subresources that have finished downloading.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Working with Frames (Legacy)

class WebFrame

A `WebFrame` object encapsulates the data displayed in a `WebFrameView` object. There is one `WebFrame` object per frame displayed in a `WebView`. An entire webpage is represented by a hierarchy of `WebFrame` objects in which the root object is called the **main frame**.

Deprecated

class WebFrameView

`WebFrameView` objects and their subviews display the web content contained in a frame. You never create instances of `WebFrameView` directly—`WebView` objects create and manage a hierarchy of `WebFrameView` objects, one for each frame. `WebFrameView` objects use a scroll view whose document view conforms to the WebDocumentView protocol.

Deprecated

protocol WebFrameLoadDelegateDeprecated

