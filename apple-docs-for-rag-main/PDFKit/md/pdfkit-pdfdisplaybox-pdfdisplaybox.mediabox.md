

- PDFKit
- PDFDisplayBox
-  PDFDisplayBox.mediaBox 

Case

# PDFDisplayBox.mediaBox

A rectangle defining the boundaries of the physical medium for display or printing, expressed in default user-space units.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.4+tvOS 11.0+visionOS 1.0+

``` source
case mediaBox
```

## See Also

### Constants

case cropBox

A rectangle defining the boundaries of the visible region , expressed in default user-space units. Default value equal to `kPDFDisplayBoxMediaBox`.

case bleedBox

A rectangle defining the boundaries of the clip region for the page contents in a production environment. Default value equal to `kPDFDisplayBoxCropBox`.

case trimBox

A rectangle defining the intended boundaries of the finished page. Default value equal to `kPDFDisplayBoxCropBox`.

case artBox

A rectangle defining the boundaries of the page’s meaningful content including surrounding white space intended for display. Default value equal to `kPDFDisplayBoxCropBox`.

