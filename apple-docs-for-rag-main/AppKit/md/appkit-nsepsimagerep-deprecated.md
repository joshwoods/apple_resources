

- AppKit
-  NSEPSImageRep Deprecated

Class

# NSEPSImageRep

An object that can render an image from encapsulated PostScript (EPS) code.

macOS 10.0–14.0Deprecated

``` source
class NSEPSImageRep
```

Deprecated

\`NSEPSImageRep\` instances cannot be created on macOS 14.0 and later

## Topics

### Creating Representations of Images from EPS Data

init?(data: Data)

Returns a representation of an image initialized with the specified EPS data.

### Getting Data

var boundingBox: NSRect

The rectangle that bounds the image representation.

var epsRepresentation: Data

The EPS representation of the image representation.

### Drawing Images

func prepareGState()

Implemented by subclasses to configure the graphics state prior to drawing.

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

class NSPDFImageRep

An object that can render an image from a PDF format data stream.

class NSPDFInfo

An object that stores information associated with the creation of a PDF file, such as its URL, tag names, page orientation, and paper size.

