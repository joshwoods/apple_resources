

- PDFKit
- PDFView
-  drawPagePost(\_:) Deprecated

Instance Method

# drawPagePost(\_:)

Perform post-page rendering.

macOS 10.5–10.12Deprecated

``` source
@MainActor
func drawPagePost(_ page: PDFPage)
```

## Discussion

The default implementation of this method draws the text highlighting (if any) for the page. This method does not apply scaling or rotating to the current context to map to page space; instead, the context is in view-space coordinates (in which the origin is at the lower-left corner of the current PDF view).

## See Also

### Rendering the View and Printing

func draw(PDFPage)

Draw and render a visible page.

Deprecated

func print(with: NSPrintInfo, autoRotate: Bool)

Prints the document with the specified printer information.

func print(with: NSPrintInfo, autoRotate: Bool, pageScaling: PDFPrintScalingMode)

Prints the document with the specified printer and page-scaling information.

