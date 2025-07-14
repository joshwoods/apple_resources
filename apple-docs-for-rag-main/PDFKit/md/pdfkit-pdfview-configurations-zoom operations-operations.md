

- PDFKit
- PDFView
- Configurations
-  Zoom Operations 

API Collection

# Zoom Operations

Zoom operations for a PDF View.

## Topics

### Zooming in a PDF View

func zoomIn(Any?)

Zooms in by increasing the scaling factor.

var canZoomIn: Bool

Returns a Boolean value indicating whether the user can magnify the view and zoom in.

func zoomOut(Any?)

Zooms out by decreasing the scaling factor.

var canZoomOut: Bool

Returns a Boolean value indicating whether the user can view an expanded area and zoom out.

## See Also

### Scaling the View

var scaleFactor: CGFloat

The current scale factor for the view.

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

