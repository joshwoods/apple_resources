

- PDFKit
- PDFView
-  rowSize(for:) 

Instance Method

# rowSize(for:)

Returns the size needed to display a row of the current document page.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.4+tvOS 11.0+visionOS 1.0+

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS**

``` source
@MainActor
func rowSize(for page: PDFPage) -> CGSize
```

**macOS**

``` source
@MainActor
func rowSize(for page: PDFPage) -> NSSize
```

## Discussion

The size is dependent on the current scale factor and display attributes.

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

Zoom Operations

Zoom operations for a PDF View.

