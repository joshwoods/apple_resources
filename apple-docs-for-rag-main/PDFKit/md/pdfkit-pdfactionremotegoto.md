

- PDFKit
-  PDFActionRemoteGoTo 

Class

# PDFActionRemoteGoTo

`PDFActionRemoteGoTo`, a subclass of `PDFAction`, defines methods for getting and setting the destination of a go-to action that targets another document.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.5+tvOS 11.0+visionOS 1.0+

``` source
class PDFActionRemoteGoTo
```

## Topics

### Initializing the Remote Go-to Action

init(pageIndex: Int, at: CGPoint, fileURL: URL)

Initializes the remote go-to action with the specified page index, point, and document URL.

### Accessing the Page Index of the Referenced Document

var pageIndex: Int

Returns the zero-based page index referenced by the remote go-to action.

### Accessing a Point on the Referenced Page

var point: CGPoint

Sets the point, in page space, on the page referenced by the remote go-to action.

### Accessing the URL of the Referenced Document

var url: URL

Returns the URL of the document referenced by the remote go-to action.

## Relationships

### Inherits From

- PDFAction

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Action Types

class PDFActionGoTo

`PDFActionGoTo`, a subclass of `PDFAction`, defines methods for getting and setting the destination of a go-to action.

class PDFActionNamed

`PDFActionNamed` defines methods used to work with actions in PDF documents, some of which are named in the Adobe PDF Specification.

class PDFActionResetForm

`PDFActionResetForm`, a subclass of `PDFAction`, defines methods for getting and clearing fields in a PDF form.

class PDFActionURL

`PDFActionURL`, a subclass of `PDFAction`, defines methods for getting and setting the URL associated with a URL action.

enum PDFActionNamedName

