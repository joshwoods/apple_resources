

- VisionKit
- ImageAnalysisOverlayView
-  setContentsRectNeedsUpdate() 

Instance Method

# setContentsRectNeedsUpdate()

Informs the view that contains the image when the layout changes and the view needs to reload its content.

macOS 13.0+

``` source
@MainActor
final func setContentsRectNeedsUpdate()
```

## Mentioned in 

Enabling Live Text interactions with images

## Discussion

The framework ignores calls to this method when the superview is of type NSImageView.

If the superview is a class other than `NSImageView`, call this method when the layout changes. The overlay view then invokes the delegate’s contentsRect(for:) method to request the new content area.

## See Also

### Managing custom image views

var contentsRect: CGRect

Returns the rectangle, in unit coordinates, that contains the image within the superview.

