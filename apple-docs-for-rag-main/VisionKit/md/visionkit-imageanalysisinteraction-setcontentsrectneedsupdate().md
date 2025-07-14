

- VisionKit
- ImageAnalysisInteraction
-  setContentsRectNeedsUpdate() 

Instance Method

# setContentsRectNeedsUpdate()

Informs the view that contains the image when the layout changes and the view needs to reload its content.

iOS 16.0+iPadOS 16.0+Mac Catalyst 17.0+visionOS 1.0+

``` source
@MainActor
final func setContentsRectNeedsUpdate()
```

## Mentioned in 

Enabling Live Text interactions with images

## Discussion

The framework ignores calls to this method when your app adds the interaction to a UIImageView, which calculates the contentsRect based on the image view’s UIView.ContentMode.

When the view that contains the image isn’t an instance of UIImageView, call this method when the layout changes. The interaction then invokes the delegate’s contentsRect(for:) callback, which provides the updated content area to the system.

## See Also

### Managing custom image views

var contentsRect: CGRect

A rectangle, in unit coordinate space, that describes the content area of the interaction.

