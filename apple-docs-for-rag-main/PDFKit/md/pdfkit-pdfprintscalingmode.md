

- PDFKit
-  PDFPrintScalingMode 

Enumeration

# PDFPrintScalingMode

The type of scaling to be used when printing a page (see PDFDocument).

macOS 10.4+

``` source
enum PDFPrintScalingMode
```

## Topics

### Enumeration Cases

case pageScaleDownToFit

Scale large pages down to fit the paper size (smaller pages do not get scaled up).

case pageScaleNone

Do not apply scaling to the page when printing.

case pageScaleToFit

Scale each page up or down to best fit the paper size.

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

### Printing Documents for macOS

func printOperation(for: NSPrintInfo?, scalingMode: PDFPrintScalingMode, autoRotate: Bool) -> NSPrintOperation?

Returns a print operation suitable for printing the PDF document.

