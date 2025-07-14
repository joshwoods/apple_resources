

- WebKit
-  WebFrame Deprecated

Class

# WebFrame

A `WebFrame` object encapsulates the data displayed in a `WebFrameView` object. There is one `WebFrame` object per frame displayed in a `WebView`. An entire webpage is represented by a hierarchy of `WebFrame` objects in which the root object is called the **main frame**.

macOS 10.3–10.14Deprecated

``` source
class WebFrame
```

## Overview

Each `WebFrame` also has a `WebDataSource` object that manages the loading of frame content. You use the load(_:) method to initiate an asynchronous client request which will create a provisional data source. The provisional data source will transition to a committed data source once any data has been received.

There are some special, predefined, frame names that you can use when referring to or finding a `WebFrame`. Some of the predefined frame names are: “\_self”, “\_current”, “\_parent”, and “\_top.” See findNamed(_:) for a description of their meaning. Frame names may also be specified in the HTML source, or set by clients.

However, the group name is an arbitrary identifier used to group related frames. For example, JavaScript running in a frame can access any other frame in the same group. It’s up to the application how it chooses to scope related frames.

## Topics

### Initializing Frames

init!(name: String!, webFrameView: WebFrameView!, webView: WebView!)

Initializes the receiver with a frame name, web frame view, and controlling web view.

### Loading Content

func load(URLRequest!)

Connects to a given URL by initiating an asynchronous client request.

func reload()

Reloads the initial request passed as an argument to load(_:).

func reloadFromOrigin()

Performs an end-to-end revalidation using cache-validating conditionals if possible.

func stopLoading()

Stops any pending loads on the receiver’s data source, and those of its children.

func loadAlternateHTMLString(String!, baseURL: URL!, forUnreachableURL: URL!)

Loads alternate content for a frame whose URL is unreachable.

func loadHTMLString(String!, baseURL: URL!)

Sets the main page contents and base URL.

func load(Data!, mimeType: String!, textEncodingName: String!, baseURL: URL!)

Sets the main page contents, MIME type, content encoding, and base URL.

func load(WebArchive!)

Loads an archive into the web frame.

### Getting the Data Source

var dataSource: WebDataSource?

The committed data source.

var provisionalDataSource: WebDataSource!

The provisional data source, or `nil` if either a load request is not in progress or a load request has completed.

### Getting Related Frames and Views

var parent: WebFrame!

The web frame’s parent web frame.

var childFrames: [Any]!

The frames of the web frame’s immediate children.

var frameView: WebFrameView!

The web frame’s view object.

var webView: WebView!

The view object that manages the web frame.

### Finding Frames

func findNamed(String!) -> WebFrame!

Returns a web frame that matches the given name.

var name: String!

The web frame’s name.

### Getting DOM Objects

var domDocument: DOMDocument!

The web frame’s DOM document.

var frameElement: DOMHTMLElement!

The web view’s DOM frame element.

var globalContext: JSGlobalContextRef!

The global JavaScript execution context for bridging between the WebKit and JavaScriptCore C API.

var javaScriptContext: JSContext!

The frame’s global JavaScript execution context.

var windowObject: WebScriptObject!

The JavaScript window object.

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

### Related Documentation

WebKit Objective-C Programming Guide

### Working with Frames (Legacy)

class WebDataSource

`WebDataSource` encapsulates the web content to be displayed in a web frame view. A `WebDataSource` object has a representation object, conforming to the `WebDocumentRepresentation` protocol, that holds the data in an appropriate format depending on the MIME type. You can extend WebKit to support new MIME types by implementing your own view and representation classes, and specifying the mapping between them using the registerClass(_:representationClass:forMIMEType:) `WebView` class method.

Deprecated

class WebFrameView

`WebFrameView` objects and their subviews display the web content contained in a frame. You never create instances of `WebFrameView` directly—`WebView` objects create and manage a hierarchy of `WebFrameView` objects, one for each frame. `WebFrameView` objects use a scroll view whose document view conforms to the WebDocumentView protocol.

Deprecated

protocol WebFrameLoadDelegateDeprecated

