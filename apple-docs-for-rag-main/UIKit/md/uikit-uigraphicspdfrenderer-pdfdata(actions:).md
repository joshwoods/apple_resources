

- UIKit
- UIGraphicsPDFRenderer
-  pdfData(actions:) 

Instance Method

# pdfData(actions:)

Creates a PDF from a set of drawing instructions and returns it as a data object.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
func pdfData(actions: (UIGraphicsPDFRendererContext) -> Void) -> Data
```

## Parameters 

`actions`  

A UIGraphicsPDFRenderer.DrawingActions block that, when invoked by the renderer, executes a set of drawing instructions to create the output PDF.

## Return Value

A Data object that contains the encoded PDF.

## Discussion

You provide a set of drawing instructions as the block argument to this method, and the method returns the resulting PDF encoded in a Data object.

You can call this method repeatedly to create multiple PDFs, each of which has identical dimensions and format.

## See Also

### Managing the PDF data

func writePDF(to: URL, withActions: (UIGraphicsPDFRendererContext) -> Void) throws

Creates a PDF from a set of drawing instructions and saves it to a specified URL.

typealias DrawingActions

A closure for drawing PDF content.

