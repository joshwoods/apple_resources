

- VisionKit
- ImageAnalysisInteraction
-  view 

Instance Property

# view

The view that uses this interaction.

iOS 16.0+iPadOS 16.0+Mac Catalyst 17.0+visionOS 1.0+

``` source
@MainActor @preconcurrency
weak final var view: UIView? { get }
```

## See Also

### Configuring an image interaction

var delegate: (any ImageAnalysisInteractionDelegate)?

The delegate that handles the interaction callbacks.

var analysis: ImageAnalysis?

The results of analyzing an image for items that people can interact with.

var preferredInteractionTypes: ImageAnalysisInteraction.InteractionTypes

The types of interactions that people can perform with the image.

struct InteractionTypes

The types of interactions that people can perform with an image.

var activeInteractionTypes: ImageAnalysisInteraction.InteractionTypes

The types of interactions that a person actively performs.

