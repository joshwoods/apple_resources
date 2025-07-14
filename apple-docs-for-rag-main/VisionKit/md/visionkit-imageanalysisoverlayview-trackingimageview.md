

- VisionKit
- ImageAnalysisOverlayView
-  trackingImageView 

Instance Property

# trackingImageView

The image view that contains the image.

macOS 13.0+

``` source
@MainActor
weak final var trackingImageView: NSImageView? { get set }
```

## Mentioned in 

Enabling Live Text interactions with images

## Discussion

Optionally, set this property to the image view that contains the image, and the overlay view automatically calculates the contentsRect property value based on the image view properties.

## See Also

### Configuring overlay views

var delegate: (any ImageAnalysisOverlayViewDelegate)?

An object that handles image analysis interface callbacks.

var analysis: ImageAnalysis?

The results of analyzing an image for items that people can interact with.

var preferredInteractionTypes: ImageAnalysisOverlayView.InteractionTypes

The types of interactions that people can perform with the image in this overlay view.

struct InteractionTypes

The types of interactions that people can perform with an image.

var activeInteractionTypes: ImageAnalysisOverlayView.InteractionTypes

The types of interactions that a person actively performs.

