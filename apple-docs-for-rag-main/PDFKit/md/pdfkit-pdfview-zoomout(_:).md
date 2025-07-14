

- PDFKit
- PDFView
-  zoomOut(\_:) 

Instance Method

# zoomOut(\_:)

Zooms out by decreasing the scaling factor.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.4+tvOS 11.0+visionOS 1.0+

``` source
@IBAction @MainActor
func zoomOut(_ sender: Any?)
```

## Discussion

Each invocation of `zoomOut` divides the scaling factor by the square root of 2.

## See Also

### Zooming in a PDF View

func zoomIn(Any?)

Zooms in by increasing the scaling factor.

var canZoomIn: Bool

Returns a Boolean value indicating whether the user can magnify the view and zoom in.

var canZoomOut: Bool

Returns a Boolean value indicating whether the user can view an expanded area and zoom out.

