

- PDFKit
- PDFView
-  print(with:autoRotate:pageScaling:) 

Instance Method

# print(with:autoRotate:pageScaling:)

Prints the document with the specified printer and page-scaling information.

macOS 10.5+

``` source
@MainActor
func print(
    with printInfo: NSPrintInfo,
    autoRotate doRotate: Bool,
    pageScaling scale: PDFPrintScalingMode
)
```

## Discussion

If `pageScaling` is set to `kPDFPrintPageScaleToFit`, each page is scaled up or down to best fit the paper size. If `pageScaling` is set to `kPDFPrintPageScaleDownToFit`, only large pages are scaled down to fit; small pages are not scaled up to fit. Specifying `kPDFPrintPageScaleNone` for `pageScaling` is equivalent to calling print(with:autoRotate:). See PDFDocument for more information on page-scaling types.

## See Also

### Rendering the View and Printing

func draw(PDFPage)

Draw and render a visible page.

Deprecated

func drawPagePost(PDFPage)

Perform post-page rendering.

Deprecated

func print(with: NSPrintInfo, autoRotate: Bool)

Prints the document with the specified printer information.

