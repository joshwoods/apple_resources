

- AppKit
-  NSPDFImageRep 

Class

# NSPDFImageRep

An object that can render an image from a PDF format data stream.

macOS

``` source
class NSPDFImageRep
```

## Topics

### Creating Representations of Images from PDF Data

init?(data: Data)

Returns a representation of an image initialized with the specified PDF data.

### Getting Data

var bounds: NSRect

The image representation’s bounding rectangle.

var currentPage: Int

The page currently displayed by the image representation.

var pageCount: Int

The number of pages in the image representation.

var pdfRepresentation: Data

The PDF representation of the representation’s image.

## Relationships

### Inherits From

- NSImageRep

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol

## See Also

### Vector Formats

class NSPDFInfo

An object that stores information associated with the creation of a PDF file, such as its URL, tag names, page orientation, and paper size.

class NSEPSImageRep

An object that can render an image from encapsulated PostScript (EPS) code.

Deprecated

