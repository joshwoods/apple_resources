

- VisionKit
- ImageAnalysisInteraction
-  preferredInteractionTypes 

Instance Property

# preferredInteractionTypes

The types of interactions that people can perform with the image.

iOS 16.0+iPadOS 16.0+Mac Catalyst 17.0+visionOS 1.0+

``` source
@MainActor
final var preferredInteractionTypes: ImageAnalysisInteraction.InteractionTypes { get set }
```

## Mentioned in 

Enabling Live Text interactions with images

## Discussion

You need to set this property to enable interactions with the image. If this property contains automatic, the interaction ignores the other types in the set. The default value for this property is an empty array that disables any interactions.

If you set this property to one or more types, the interaction sets the view’s isUserInteractionEnabled property to `true` so that the interaction begins. For example, when you’re ready to start the Live Text interface, set this property to automatic.

If you set this property to an empty array, the image analysis interaction doesn’t reset the view’s `isUserInteractionEnabled` property to `false`.

## See Also

### Configuring an image interaction

var delegate: (any ImageAnalysisInteractionDelegate)?

The delegate that handles the interaction callbacks.

var analysis: ImageAnalysis?

The results of analyzing an image for items that people can interact with.

var view: UIView?

The view that uses this interaction.

struct InteractionTypes

The types of interactions that people can perform with an image.

var activeInteractionTypes: ImageAnalysisInteraction.InteractionTypes

The types of interactions that a person actively performs.

