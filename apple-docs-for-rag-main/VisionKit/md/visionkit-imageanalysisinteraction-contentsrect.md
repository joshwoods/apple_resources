

- VisionKit
- ImageAnalysisInteraction
-  contentsRect 

Instance Property

# contentsRect

A rectangle, in unit coordinate space, that describes the content area of the interaction.

iOS 16.0+iPadOS 16.0+Mac Catalyst 17.0+visionOS 1.0+

``` source
@MainActor
final var contentsRect: CGRect { get }
```

## Discussion

If the interaction’s view isn’t an instance of UIImageView, your app sets the value for this property by implementing the ImageAnalysisInteractionDelegate callback contentsRect(for:). The default return value is the unit rectangle, `[0.0, 0.0, 1.0, 1.0]`, which represents the whole view contents.

## See Also

### Managing custom image views

func setContentsRectNeedsUpdate()

Informs the view that contains the image when the layout changes and the view needs to reload its content.

