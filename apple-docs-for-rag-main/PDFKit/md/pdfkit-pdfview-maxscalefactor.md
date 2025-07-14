

- PDFKit
- PDFView
-  maxScaleFactor 

Instance Property

# maxScaleFactor

The maximum scaling factor for the PDF document.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
@MainActor
var maxScaleFactor: CGFloat { get set }
```

## See Also

### Scaling the View

var scaleFactor: CGFloat

The current scale factor for the view.

var scaleFactorForSizeToFit: CGFloat

The “size to fit” scale factor that `autoScales` would use for scaling the current document and layout.

var minScaleFactor: CGFloat

The minimum scaling factor for the PDF document.

var autoScales: Bool

A Boolean value indicating whether autoscaling is set.

func rowSize(for: PDFPage) -> CGSize

Returns the size needed to display a row of the current document page.

Zoom Operations

Zoom operations for a PDF View.

