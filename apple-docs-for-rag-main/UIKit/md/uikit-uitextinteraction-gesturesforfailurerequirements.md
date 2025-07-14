

- UIKit
- UITextInteraction
-  gesturesForFailureRequirements 

Instance Property

# gesturesForFailureRequirements

The list of gestures that the text interaction adds to the view hierarchy.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var gesturesForFailureRequirements: [UIGestureRecognizer] { get }
```

## Discussion

If your app provides other gestures in the same view hierarchy, you may want to set up failure requirements between your app’s gestures and the gestures added by the text interaction. To do this, use the require(toFail:) method to relate your gestures to those listed in gesturesForFailureRequirements.

## See Also

### Getting interaction information

var textInteractionMode: UITextInteractionMode

The mode of the text interaction.

enum UITextInteractionMode

Modes that determine the selection behaviors that a text interaction provides.

