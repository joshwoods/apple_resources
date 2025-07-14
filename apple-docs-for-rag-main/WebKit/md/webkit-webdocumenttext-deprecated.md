

- WebKit
-  WebDocumentText Deprecated

Protocol

# WebDocumentText

`WebDocumentText` is an optional protocol for document view objects that display text. This protocol defines methods for accessing document content as strings, and methods for text selection. Classes that adopt this protocol should also adopt WebDocumentView and inherit from `NSView`.

macOS 10.3–10.14Deprecated

``` source
protocol WebDocumentText : NSObjectProtocol
```

## Topics

### Getting document content

func string() -> String!

Returns the entire content of the web document as a string.

**Required**

func attributedString() -> NSAttributedString!

Returns the entire content of the web document as an attributed string.

**Required**

### Selecting and deselecting text

func selectAll()

Selects all the text in the web document.

**Required**

func deselectAll()

Deselects the currently selected text in the web document.

**Required**

func selectedString() -> String!

Returns the currently selected text in the web document as a string.

**Required**

func selectedAttributedString() -> NSAttributedString!

Returns the currently selected text in the web document as an attributed string.

**Required**

### Text encoding

func supportsTextEncoding() -> Bool

Returns a Boolean value that indicates whether the web document supports text encoding.

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

protocol WebDocumentView

This protocol is adopted by the document view of a `WebFrameView`. You can extend WebKit to support additional MIME types by implementing your own document view and document representation classes to render data for specific MIME types. You register those classes using the WebFrame registerClass(_:representationClass:forMIMEType:) method. Classes that adopt this protocol are expected to be subclasses of `NSView`.

Deprecated

