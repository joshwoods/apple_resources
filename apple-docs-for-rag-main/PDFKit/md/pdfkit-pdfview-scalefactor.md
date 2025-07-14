

- PDFKit
- PDFView
-  scaleFactor 

Instance Property

# scaleFactor

The current scale factor for the view.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.4+tvOS 11.0+visionOS 1.0+

``` source
@MainActor
var scaleFactor: CGFloat { get set }
```

## See Also

### Scaling the View

var scaleFactorForSizeToFit: CGFloat

The “size to fit” scale factor that `autoScales` would use for scaling the current document and layout.

var maxScaleFactor: CGFloat

The maximum scaling factor for the PDF document.

var minScaleFactor: CGFloat

The minimum scaling factor for the PDF document.

var autoScales: Bool

A Boolean value indicating whether autoscaling is set.

func rowSize(for: PDFPage) -> CGSize

Returns the size needed to display a row of the current document page.

Zoom Operations

Zoom operations for a PDF View.

