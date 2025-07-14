

- PDFKit
- PDFView
-  draw(\_:) Deprecated

Instance Method

# draw(\_:)

Draw and render a visible page.

macOS 10.4–10.12Deprecated

``` source
@MainActor
func draw(_ page: PDFPage)
```

## Discussion

Do not invoke this method, except by invoking it on `super` from a subclass.

The `PDFView` class calls draw(_:) as necessary for each visible page that requires rendering. In the `PDFView` class, this method erases `page` to white, calls `[page drawInRect: pageRect withBox: [self displayBox]]` , and then draws the selection, if any.

You can override this method to draw on top of a PDF page or to control how pages are drawn. In these cases, invoke this method on `super` and then perform custom drawing on top of the PDF page.

## See Also

### Rendering the View and Printing

func drawPagePost(PDFPage)

Perform post-page rendering.

Deprecated

func print(with: NSPrintInfo, autoRotate: Bool)

Prints the document with the specified printer information.

func print(with: NSPrintInfo, autoRotate: Bool, pageScaling: PDFPrintScalingMode)

Prints the document with the specified printer and page-scaling information.

