

- UIKit
- UIDragInteractionDelegate
-  dragInteraction(\_:previewForLifting:session:) 

Instance Method

# dragInteraction(\_:previewForLifting:session:)

Asks the delegate for the targeted drag item preview that will appear during the lift animation.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func dragInteraction(
    _ interaction: UIDragInteraction,
    previewForLifting item: UIDragItem,
    session: any UIDragSession
) -> UITargetedDragPreview?
```

## Parameters 

`interaction`  

The interaction that called this method.

`item`  

The drag item represented by the preview.

`session`  

The current drag session.

## Return Value

A targeted drag item preview you create, or `nil` to tell the system not to display the lift animation.

## Discussion

If you don’t provide this method, the system creates a preview based on the view owned by the drag interaction.

## See Also

### Providing drag previews

func dragInteraction(UIDragInteraction, previewForCancelling: UIDragItem, withDefault: UITargetedDragPreview) -> UITargetedDragPreview?

Asks the delegate for the targeted drag item preview to show during the cancellation animation.

func dragInteraction(UIDragInteraction, prefersFullSizePreviewsFor: any UIDragSession) -> Bool

Asks the delegate whether the preview should appear in its original size or a scaled size.

