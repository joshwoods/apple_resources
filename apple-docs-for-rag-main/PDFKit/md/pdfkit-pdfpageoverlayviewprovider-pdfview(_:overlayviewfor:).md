

- PDFKit
- PDFPageOverlayViewProvider
-  pdfView(\_:overlayViewFor:) 

Instance Method

# pdfView(\_:overlayViewFor:)

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

**macOS**

``` source
func pdfView(
    _ view: PDFView,
    overlayViewFor page: PDFPage
) -> NSView?
```

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS**

``` source
func pdfView(
    _ view: PDFView,
    overlayViewFor page: PDFPage
) -> UIView?
```

**Required**

## See Also

### Instance Methods

func pdfView(PDFView, willDisplayOverlayView: UIView, for: PDFPage)

func pdfView(PDFView, willEndDisplayingOverlayView: UIView, for: PDFPage)

