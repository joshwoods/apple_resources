

- Core Graphics
- CGPDFPage
-  getBoxRect(\_:) 

Instance Method

# getBoxRect(\_:)

Returns the rectangle that represents a type of box for a content region or page dimensions of a PDF page.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.3+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func getBoxRect(_ box: CGPDFBox) -> CGRect
```

## Parameters 

`box`  

A constant that specifies the type of box. For possible values, see CGPDFBox.

## Return Value

Returns the rectangle associated with the type of box specified by the `box` parameter in the specified page.

## Discussion

Returns the rectangle associated with the specified box in the specified page. This is the value of the corresponding entry (such as `/MediaBox`, `/ArtBox`, and so on) in the page’s dictionary.

## See Also

### Getting Page Information

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

