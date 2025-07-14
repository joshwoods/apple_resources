

- WebKit
-  WebDocumentRepresentation Deprecated

Protocol

# WebDocumentRepresentation

This protocol is adopted by document representation classes that handle specific MIME types. You can implement your own document view classes and document representation classes to render data for specific MIME types, and register those classes using the `WebFrame` registerClass(_:representationClass:forMIMEType:) method.

macOS 10.3–10.14Deprecated

``` source
protocol WebDocumentRepresentation : NSObjectProtocol
```

## Topics

### Setting the data source

func setDataSource(WebDataSource!)

Sets the receiver’s data source.

**Required**

### Loading content

func receivedData(Data!, with: WebDataSource!)

Invoked when a data source has received some data.

**Required**

func receivedError((any Error)!, with: WebDataSource!)

Invoked when a data source receives an error loading its content.

**Required**

func finishedLoading(with: WebDataSource!)

Invoked when a data source finishes loading its content.

**Required**

### Getting document source

func canProvideDocumentSource() -> Bool

Returns whether the receiver can provide content source.

**Required**

func documentSource() -> String!

Returns the receiver’s source as text.

**Required**

### Getting the document title

func title() -> String!

Returns the receiver’s document title.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Working With Document Web Views (Legacy)

protocol WebDocumentSearching

`WebDocumentSearching` is an optional protocol for document view objects that support searching. Classes that adopt this protocol should also adopt `WebDocumentView` and inherit from `NSView`.

Deprecated

protocol WebDocumentText

`WebDocumentText` is an optional protocol for document view objects that display text. This protocol defines methods for accessing document content as strings, and methods for text selection. Classes that adopt this protocol should also adopt WebDocumentView and inherit from `NSView`.

Deprecated

protocol WebDocumentView

This protocol is adopted by the document view of a `WebFrameView`. You can extend WebKit to support additional MIME types by implementing your own document view and document representation classes to render data for specific MIME types. You register those classes using the WebFrame registerClass(_:representationClass:forMIMEType:) method. Classes that adopt this protocol are expected to be subclasses of `NSView`.

Deprecated

