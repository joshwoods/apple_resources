

- Core Graphics
- CGPDFPage
-  document 

Instance Property

# document

Returns the document for a page.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.3+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var document: CGPDFDocument? { get }
```

## See Also

### Getting Page Information

func getBoxRect(CGPDFBox) -> CGRect

Returns the rectangle that represents a type of box for a content region or page dimensions of a PDF page.

var dictionary: CGPDFDictionaryRef?

Returns the dictionary of a PDF page.

var pageNumber: Int

Returns the page number of the specified PDF page.

var rotationAngle: Int32

Returns the rotation angle of a PDF page, in degrees.

func getDrawingTransform(CGPDFBox, rect: CGRect, rotate: Int32, preserveAspectRatio: Bool) -> CGAffineTransform

Returns the affine transform that maps a box to a given rectangle on a PDF page.

