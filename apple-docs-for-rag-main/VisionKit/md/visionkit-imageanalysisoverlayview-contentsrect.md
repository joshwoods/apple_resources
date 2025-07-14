

- VisionKit
- ImageAnalysisOverlayView
-  contentsRect 

Instance Property

# contentsRect

Returns the rectangle, in unit coordinates, that contains the image within the superview.

macOS 13.0+

``` source
@MainActor
final var contentsRect: CGRect { get }
```

## Discussion

If your app displays the image with NSImageView and you assign it to the trackingImageView property, the framework doesn’t require you to implement this property.

The default value is the entire contents of the superview, which is the unit rectangle `[0.0, 0.0, 1.0, 1.0]`.

## See Also

### Managing custom image views

func setContentsRectNeedsUpdate()

Informs the view that contains the image when the layout changes and the view needs to reload its content.

