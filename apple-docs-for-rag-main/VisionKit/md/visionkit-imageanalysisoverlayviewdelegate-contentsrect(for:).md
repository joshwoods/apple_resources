

- VisionKit
- ImageAnalysisOverlayViewDelegate
-  contentsRect(for:) 

Instance Method

# contentsRect(for:)

Returns the rectangle, in unit coordinate space, that contains the image within the view.

macOS 13.0+

``` source
@MainActor
func contentsRect(for overlayView: ImageAnalysisOverlayView) -> CGRect
```

**Required** Default implementation provided.

## Parameters 

`overlayView`  

The associated overlay view for the contents rectangle.

## Return Value

The rectangle of the image within the view, in unit coordinates. The default return value is the unit rectangle `[0.0, 0.0, 1.0, 1.0]`, which represents the whole view contents.

## Discussion

Implement this method if the trackingImageView type isn’t NSImageView.

## Default Implementations

### ImageAnalysisOverlayViewDelegate Implementations

func contentsRect(for: ImageAnalysisOverlayView) -> CGRect

A default implementation that returns a rectangle that specifies the full width and height of the view.

## See Also

### Providing interface details

func contentView(for: ImageAnalysisOverlayView) -> NSView?

Provides the view that contains the image.

**Required** Default implementation provided.

