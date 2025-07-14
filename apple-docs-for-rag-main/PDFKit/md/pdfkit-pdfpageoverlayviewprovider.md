

- PDFKit
-  PDFPageOverlayViewProvider 

Protocol

# PDFPageOverlayViewProvider

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
protocol PDFPageOverlayViewProvider : NSObjectProtocol
```

## Topics

### Instance Methods

func pdfView(PDFView, overlayViewFor: PDFPage) -> UIView?

**Required**

func pdfView(PDFView, willDisplayOverlayView: UIView, for: PDFPage)

func pdfView(PDFView, willEndDisplayingOverlayView: UIView, for: PDFPage)

## Relationships

### Inherits From

- NSObjectProtocol

