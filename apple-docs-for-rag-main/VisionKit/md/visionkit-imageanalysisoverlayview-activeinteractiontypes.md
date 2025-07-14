

- VisionKit
- ImageAnalysisOverlayView
-  activeInteractionTypes 

Instance Property

# activeInteractionTypes

The types of interactions that a person actively performs.

macOS 13.0+

``` source
@MainActor
final var activeInteractionTypes: ImageAnalysisOverlayView.InteractionTypes { get }
```

## Discussion

This property is always a concrete type that’s never set to automatic.

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

var trackingImageView: NSImageView?

The image view that contains the image.

