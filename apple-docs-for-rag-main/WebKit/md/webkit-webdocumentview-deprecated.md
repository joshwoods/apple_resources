

- WebKit
-  WebDocumentView Deprecated

Protocol

# WebDocumentView

This protocol is adopted by the document view of a `WebFrameView`. You can extend WebKit to support additional MIME types by implementing your own document view and document representation classes to render data for specific MIME types. You register those classes using the WebFrame registerClass(_:representationClass:forMIMEType:) method. Classes that adopt this protocol are expected to be subclasses of `NSView`.

macOS 10.3–10.14Deprecated

``` source
protocol WebDocumentView : NSObjectProtocol
```

## Topics

### Setting the data source

func setDataSource(WebDataSource!)

Invoked when the data source for this document has been changed.

**Required**

func dataSourceUpdated(WebDataSource!)

Invoked when additional data has been received.

**Required**

### Controlling the layout

func setNeedsLayout(Bool)

Sets whether or not the receiver should change its layout.

**Required**

func layout()

Invoked when the receiver should change its layout immediately.

**Required**

### Attaching to a window

func viewDidMoveToHostWindow()

Invoked when a web view’s host window is set.

**Required**

func viewWillMove(toHostWindow: NSWindow!)

Invoked when a web view’s host window is about to change.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Working With Document Web Views (Legacy)

protocol WebDocumentRepresentation

This protocol is adopted by document representation classes that handle specific MIME types. You can implement your own document view classes and document representation classes to render data for specific MIME types, and register those classes using the `WebFrame` registerClass(_:representationClass:forMIMEType:) method.

Deprecated

protocol WebDocumentSearching

`WebDocumentSearching` is an optional protocol for document view objects that support searching. Classes that adopt this protocol should also adopt `WebDocumentView` and inherit from `NSView`.

Deprecated

protocol WebDocumentText

`WebDocumentText` is an optional protocol for document view objects that display text. This protocol defines methods for accessing document content as strings, and methods for text selection. Classes that adopt this protocol should also adopt WebDocumentView and inherit from `NSView`.

Deprecated

