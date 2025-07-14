

- VisionKit
- ImageAnalysisOverlayView
-  preferredInteractionTypes 

Instance Property

# preferredInteractionTypes

The types of interactions that people can perform with the image in this overlay view.

macOS 13.0+

``` source
@MainActor
final var preferredInteractionTypes: ImageAnalysisOverlayView.InteractionTypes { get set }
```

## Mentioned in 

Enabling Live Text interactions with images

## Discussion

You need to set this property to enable the Live Text interface with the image. If this property contains automatic, the overlay view ignores the other interaction types in the set. The default value for this property is an empty array that disables any interactions.

## See Also

### Configuring overlay views

var delegate: (any ImageAnalysisOverlayViewDelegate)?

An object that handles image analysis interface callbacks.

var analysis: ImageAnalysis?

The results of analyzing an image for items that people can interact with.

struct InteractionTypes

The types of interactions that people can perform with an image.

var trackingImageView: NSImageView?

The image view that contains the image.

var activeInteractionTypes: ImageAnalysisOverlayView.InteractionTypes

The types of interactions that a person actively performs.

