

- PDFKit
- PDFPageOverlayViewProvider
-  pdfView(\_:willEndDisplayingOverlayView:for:) 

Instance Method

# pdfView(\_:willEndDisplayingOverlayView:for:)

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

**macOS**

``` source
optional func pdfView(
    _ pdfView: PDFView,
    willEndDisplayingOverlayView overlayView: NSView,
    for page: PDFPage
)
```

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS**

``` source
optional func pdfView(
    _ pdfView: PDFView,
    willEndDisplayingOverlayView overlayView: UIView,
    for page: PDFPage
)
```

## See Also

### Instance Methods

func pdfView(PDFView, overlayViewFor: PDFPage) -> UIView?

**Required**

func pdfView(PDFView, willDisplayOverlayView: UIView, for: PDFPage)

