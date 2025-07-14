

- UIKit
- UIPreviewInteractionDelegate
-  previewInteraction(\_:didUpdatePreviewTransition:ended:) 

Instance Method

# previewInteraction(\_:didUpdatePreviewTransition:ended:)

Informs the delegate of the progress through the preview phase of the preview interaction.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func previewInteraction(
    _ previewInteraction: UIPreviewInteraction,
    didUpdatePreviewTransition transitionProgress: CGFloat,
    ended: Bool
)
```

**Required**

## Parameters 

`previewInteraction`  

The preview interaction associated with the current user input.

`transitionProgress`  

The progress through the preview phase of the transition. A CGFloat with a value from `0` to `1`.

`ended`  

A Boolean whose value indicates whether the preview phase of the transition is complete.

## Discussion

This method is called repeatedly during the preview phase of the preview interaction. Use the supplied `transitionProgress` parameter to update the UI to reflect the progress of the interaction. For example, the *peek* effect in view controller preview transitions progressively blurs everything except the appropriate view.

The `ended` parameter is false throughout the preview phase and becomes true as the phase is completed. The preview interaction then transitions to the commit phase, so you should use this point to update the UI as required.

## See Also

### Managing preview interactions

func previewInteractionShouldBegin(UIPreviewInteraction) -> Bool

Asks the delegate whether a preview interaction is allowed to begin.

func previewInteraction(UIPreviewInteraction, didUpdateCommitTransition: CGFloat, ended: Bool)

Informs the delegate of the preview interaction’s progress through the commit phase.

func previewInteractionDidCancel(UIPreviewInteraction)

Informs the delegate that the specified preview interaction was canceled.

**Required**

