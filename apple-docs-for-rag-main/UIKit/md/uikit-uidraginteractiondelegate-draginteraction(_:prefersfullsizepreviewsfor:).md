

- UIKit
- UIDragInteractionDelegate
-  dragInteraction(\_:prefersFullSizePreviewsFor:) 

Instance Method

# dragInteraction(\_:prefersFullSizePreviewsFor:)

Asks the delegate whether the preview should appear in its original size or a scaled size.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func dragInteraction(
    _ interaction: UIDragInteraction,
    prefersFullSizePreviewsFor session: any UIDragSession
) -> Bool
```

## Parameters 

`interaction`  

The interaction that called this method.

`session`  

The current drag session.

## Return Value

true to tell the system the preview should appear in its original size; otherwise false, which is the default if you don’t provide this method.

## Discussion

The return value is a recommendation to the system. The system may choose to scale the preview to a smaller size, according to its own rules, even if you return true.

## See Also

### Providing drag previews

func dragInteraction(UIDragInteraction, previewForLifting: UIDragItem, session: any UIDragSession) -> UITargetedDragPreview?

Asks the delegate for the targeted drag item preview that will appear during the lift animation.

func dragInteraction(UIDragInteraction, previewForCancelling: UIDragItem, withDefault: UITargetedDragPreview) -> UITargetedDragPreview?

Asks the delegate for the targeted drag item preview to show during the cancellation animation.

