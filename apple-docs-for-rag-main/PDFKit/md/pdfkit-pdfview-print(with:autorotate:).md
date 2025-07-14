

- PDFKit
- PDFView
-  print(with:autoRotate:) 

Instance Method

# print(with:autoRotate:)

Prints the document with the specified printer information.

macOS 10.4+

``` source
@MainActor
func print(
    with printInfo: NSPrintInfo,
    autoRotate doRotate: Bool
)
```

## Discussion

If `autoRotate` is set to true, then ths method ignores the orientation attribute in the `NSPrintInfo` object and instead chooses the orientation that best fits the page to the paper size. This orientation occurs on a page-by-page basis.

## See Also

### Rendering the View and Printing

func draw(PDFPage)

Draw and render a visible page.

Deprecated

func drawPagePost(PDFPage)

Perform post-page rendering.

Deprecated

func print(with: NSPrintInfo, autoRotate: Bool, pageScaling: PDFPrintScalingMode)

Prints the document with the specified printer and page-scaling information.

