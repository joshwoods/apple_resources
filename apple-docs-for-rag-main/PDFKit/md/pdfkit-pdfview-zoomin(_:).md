

- PDFKit
- PDFView
-  zoomIn(\_:) 

Instance Method

# zoomIn(\_:)

Zooms in by increasing the scaling factor.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.4+tvOS 11.0+visionOS 1.0+

``` source
@IBAction @MainActor
func zoomIn(_ sender: Any?)
```

## Discussion

Each invocation of `zoomIn` muliplies the scaling factor by the square root of 2.

## See Also

### Zooming in a PDF View

var canZoomIn: Bool

Returns a Boolean value indicating whether the user can magnify the view and zoom in.

func zoomOut(Any?)

Zooms out by decreasing the scaling factor.

var canZoomOut: Bool

Returns a Boolean value indicating whether the user can view an expanded area and zoom out.

