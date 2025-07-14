

- VisionKit
- ImageAnalysisOverlayView
-  analysis 

Instance Property

# analysis

The results of analyzing an image for items that people can interact with.

macOS 13.0+

``` source
@MainActor
final var analysis: ImageAnalysis? { get set }
```

## Mentioned in 

Enabling Live Text interactions with images

## See Also

### Configuring overlay views

var delegate: (any ImageAnalysisOverlayViewDelegate)?

An object that handles image analysis interface callbacks.

var preferredInteractionTypes: ImageAnalysisOverlayView.InteractionTypes

The types of interactions that people can perform with the image in this overlay view.

struct InteractionTypes

The types of interactions that people can perform with an image.

var trackingImageView: NSImageView?

The image view that contains the image.

var activeInteractionTypes: ImageAnalysisOverlayView.InteractionTypes

The types of interactions that a person actively performs.

