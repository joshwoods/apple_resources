

- UIKit
- UIGraphicsPDFRenderer
-  writePDF(to:withActions:) 

Instance Method

# writePDF(to:withActions:)

Creates a PDF from a set of drawing instructions and saves it to a specified URL.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
func writePDF(
    to url: URL,
    withActions actions: (UIGraphicsPDFRendererContext) -> Void
) throws
```

## Parameters 

`url`  

The URL where the complete PDF file is saved.

`actions`  

A UIGraphicsPDFRenderer.DrawingActions closure that, when invoked by the renderer, executes a set of drawing instructions to create the output PDF.

## Discussion

You provide a set of drawing instructions as the block argument to this method, and the method attempts to write the resulting PDF to the supplied URL.

You can call this method repeatedly to create multiple PDFs, each of which has identical dimensions and format.

## See Also

### Managing the PDF data

func pdfData(actions: (UIGraphicsPDFRendererContext) -> Void) -> Data

Creates a PDF from a set of drawing instructions and returns it as a data object.

typealias DrawingActions

A closure for drawing PDF content.

