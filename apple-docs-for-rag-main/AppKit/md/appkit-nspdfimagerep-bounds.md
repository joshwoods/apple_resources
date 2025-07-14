

- AppKit
- NSPDFImageRep
-  bounds 

Instance Property

# bounds

The image representation’s bounding rectangle.

macOS

``` source
var bounds: NSRect { get }
```

## Discussion

This value is equivalent to the crop box specified by the PDF data.

## See Also

### Getting Data

var currentPage: Int

The page currently displayed by the image representation.

var pageCount: Int

The number of pages in the image representation.

var pdfRepresentation: Data

The PDF representation of the representation’s image.

