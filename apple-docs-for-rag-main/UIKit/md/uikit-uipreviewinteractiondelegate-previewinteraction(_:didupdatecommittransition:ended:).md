

- UIKit
- UIPreviewInteractionDelegate
-  previewInteraction(\_:didUpdateCommitTransition:ended:) 

Instance Method

# previewInteraction(\_:didUpdateCommitTransition:ended:)

Informs the delegate of the preview interaction’s progress through the commit phase.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func previewInteraction(
    _ previewInteraction: UIPreviewInteraction,
    didUpdateCommitTransition transitionProgress: CGFloat,
    ended: Bool
)
```

## Parameters 

`previewInteraction`  

The preview interaction associated with the current user input.

`transitionProgress`  

The progress through the commit phase of the transition. A CGFloat with a value from `0` to `1`.

`ended`  

A `Boolean` whose value indicates whether the commit phase of the transition is complete.

## Discussion

This method is called repeatedly during the commit phase of the preview interaction. Use the supplied `transitionProgress` parameter to update the UI to reflect the progress of the interaction. For example, the *pop* effect in view controller preview transitions progressively increases the size of the child view controller as the transition progresses.

The `ended` parameter is false throughout the commit phase and becomes true when the phase is completed. At this point, the preview interaction is complete, and you should update the UI appropriately. For example, in view controller preview interactions, the child view controller becomes the main view controller.

## See Also

### Managing preview interactions

func previewInteractionShouldBegin(UIPreviewInteraction) -> Bool

Asks the delegate whether a preview interaction is allowed to begin.

func previewInteraction(UIPreviewInteraction, didUpdatePreviewTransition: CGFloat, ended: Bool)

Informs the delegate of the progress through the preview phase of the preview interaction.

**Required**

func previewInteractionDidCancel(UIPreviewInteraction)

Informs the delegate that the specified preview interaction was canceled.

**Required**

