

- PDFKit
- PDFPageOverlayViewProvider
-  pdfView(\_:willDisplayOverlayView:for:) 

Instance Method

# pdfView(\_:willDisplayOverlayView:for:)

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

**macOS**

``` source
optional func pdfView(
    _ pdfView: PDFView,
    willDisplayOverlayView overlayView: NSView,
    for page: PDFPage
)
```

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS**

``` source
optional func pdfView(
    _ pdfView: PDFView,
    willDisplayOverlayView overlayView: UIView,
    for page: PDFPage
)
```

## See Also

### Instance Methods

func pdfView(PDFView, overlayViewFor: PDFPage) -> UIView?

**Required**

func pdfView(PDFView, willEndDisplayingOverlayView: UIView, for: PDFPage)

