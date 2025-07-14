

- VisionKit
- ImageAnalysisInteraction
-  delegate 

Instance Property

# delegate

The delegate that handles the interaction callbacks.

iOS 16.0+iPadOS 16.0+Mac Catalyst 17.0+visionOS 1.0+

``` source
@MainActor
weak final var delegate: (any ImageAnalysisInteractionDelegate)? { get set }
```

## See Also

### Configuring an image interaction

var analysis: ImageAnalysis?

The results of analyzing an image for items that people can interact with.

var view: UIView?

The view that uses this interaction.

var preferredInteractionTypes: ImageAnalysisInteraction.InteractionTypes

The types of interactions that people can perform with the image.

struct InteractionTypes

The types of interactions that people can perform with an image.

var activeInteractionTypes: ImageAnalysisInteraction.InteractionTypes

The types of interactions that a person actively performs.

