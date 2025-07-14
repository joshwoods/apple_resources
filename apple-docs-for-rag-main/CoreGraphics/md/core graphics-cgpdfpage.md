

- Core Graphics
-  CGPDFPage 

Class

# CGPDFPage

A type that represents a page in a PDF document.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class CGPDFPage
```

## Topics

### Getting Page Information

func getBoxRect(CGPDFBox) -> CGRect

Returns the rectangle that represents a type of box for a content region or page dimensions of a PDF page.

var dictionary: CGPDFDictionaryRef?

Returns the dictionary of a PDF page.

var document: CGPDFDocument?

Returns the document for a page.

var pageNumber: Int

Returns the page number of the specified PDF page.

var rotationAngle: Int32

Returns the rotation angle of a PDF page, in degrees.

func getDrawingTransform(CGPDFBox, rect: CGRect, rotate: Int32, preserveAspectRatio: Bool) -> CGAffineTransform

Returns the affine transform that maps a box to a given rectangle on a PDF page.

### Working with Core Foundation Types

class var typeID: CFTypeID

Returns the CFType ID for PDF page objects.

### Constants

enum CGPDFBox

Box types for a PDF page.

## Relationships

### Conforms To

- Equatable
- Hashable

## See Also

### Related Documentation

Quartz 2D Programming Guide

