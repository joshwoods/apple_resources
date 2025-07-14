

- PDFKit
-  PDFActionNamedName 

Enumeration

# PDFActionNamedName

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.5+tvOS 11.0+visionOS 1.0+

``` source
enum PDFActionNamedName
```

## Topics

### Constants

case find

The Find action.

case firstPage

The First Page action.

case goBack

The Go Back action.

case goForward

The Go Forward action.

case goToPage

The Go to Page action.

case lastPage

The Last Page action.

case nextPage

The Next Page action.

case none

The action has no name.

case previousPage

The Previous Page action.

case print

The Print action.

case zoomIn

The Zoom In action.

case zoomOut

The Zoom Out action.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Action Types

class PDFActionGoTo

`PDFActionGoTo`, a subclass of `PDFAction`, defines methods for getting and setting the destination of a go-to action.

class PDFActionNamed

`PDFActionNamed` defines methods used to work with actions in PDF documents, some of which are named in the Adobe PDF Specification.

class PDFActionRemoteGoTo

`PDFActionRemoteGoTo`, a subclass of `PDFAction`, defines methods for getting and setting the destination of a go-to action that targets another document.

class PDFActionResetForm

`PDFActionResetForm`, a subclass of `PDFAction`, defines methods for getting and clearing fields in a PDF form.

class PDFActionURL

`PDFActionURL`, a subclass of `PDFAction`, defines methods for getting and setting the URL associated with a URL action.

