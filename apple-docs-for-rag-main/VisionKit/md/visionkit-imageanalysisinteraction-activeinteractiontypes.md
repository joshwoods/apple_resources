

- VisionKit
- ImageAnalysisInteraction
-  activeInteractionTypes 

Instance Property

# activeInteractionTypes

The types of interactions that a person actively performs.

iOS 16.0+iPadOS 16.0+Mac Catalyst 17.0+visionOS 1.0+

``` source
@MainActor
final var activeInteractionTypes: ImageAnalysisInteraction.InteractionTypes { get }
```

## Discussion

This property is always a concrete type that’s never set to automatic.

## See Also

### Configuring an image interaction

var delegate: (any ImageAnalysisInteractionDelegate)?

The delegate that handles the interaction callbacks.

var analysis: ImageAnalysis?

The results of analyzing an image for items that people can interact with.

var view: UIView?

The view that uses this interaction.

var preferredInteractionTypes: ImageAnalysisInteraction.InteractionTypes

The types of interactions that people can perform with the image.

struct InteractionTypes

The types of interactions that people can perform with an image.

