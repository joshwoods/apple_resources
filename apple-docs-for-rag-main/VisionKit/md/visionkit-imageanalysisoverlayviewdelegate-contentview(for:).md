

- VisionKit
- ImageAnalysisOverlayViewDelegate
-  contentView(for:) 

Instance Method

# contentView(for:)

Provides the view that contains the image.

macOS 13.0+

``` source
@MainActor
func contentView(for overlayView: ImageAnalysisOverlayView) -> NSView?
```

**Required** Default implementation provided.

## Parameters 

`overlayView`  

The associated overlay view for the content view.

## Return Value

The view that contains the image.

## Discussion

The default value is `nil`.

## Default Implementations

### ImageAnalysisOverlayViewDelegate Implementations

func contentView(for: ImageAnalysisOverlayView) -> NSView?

A default implementation that returns a `nil` reference.

## See Also

### Providing interface details

func contentsRect(for: ImageAnalysisOverlayView) -> CGRect

Returns the rectangle, in unit coordinate space, that contains the image within the view.

**Required** Default implementation provided.

