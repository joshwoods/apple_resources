

- VisionKit
- ImageAnalysisOverlayView
-  delegate 

Instance Property

# delegate

An object that handles image analysis interface callbacks.

macOS 13.0+

``` source
@MainActor
weak final var delegate: (any ImageAnalysisOverlayViewDelegate)? { get set }
```

## See Also

### Configuring overlay views

var analysis: ImageAnalysis?

The results of analyzing an image for items that people can interact with.

var preferredInteractionTypes: ImageAnalysisOverlayView.InteractionTypes

The types of interactions that people can perform with the image in this overlay view.

struct InteractionTypes

The types of interactions that people can perform with an image.

var trackingImageView: NSImageView?

The image view that contains the image.

var activeInteractionTypes: ImageAnalysisOverlayView.InteractionTypes

The types of interactions that a person actively performs.

