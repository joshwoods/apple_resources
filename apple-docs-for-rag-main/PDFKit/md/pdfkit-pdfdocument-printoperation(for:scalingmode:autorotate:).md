

- PDFKit
- PDFDocument
-  printOperation(for:scalingMode:autoRotate:) 

Instance Method

# printOperation(for:scalingMode:autoRotate:)

Returns a print operation suitable for printing the PDF document.

macOS 10.7+

``` source
func printOperation(
    for printInfo: NSPrintInfo?,
    scalingMode scaleMode: PDFPrintScalingMode,
    autoRotate doRotate: Bool
) -> NSPrintOperation?
```

## See Also

### Printing Documents for macOS

enum PDFPrintScalingMode

The type of scaling to be used when printing a page (see PDFDocument).

