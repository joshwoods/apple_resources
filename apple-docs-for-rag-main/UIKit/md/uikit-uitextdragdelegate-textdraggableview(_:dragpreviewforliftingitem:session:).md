

- UIKit
- UITextDragDelegate
-  textDraggableView(\_:dragPreviewForLiftingItem:session:) 

Instance Method

# textDraggableView(\_:dragPreviewForLiftingItem:session:)

Asks the delegate for the preview to show during the lift animation that happens when a user begins to drag an item from a text view.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func textDraggableView(
    _ textDraggableView: any UIView & UITextDraggable,
    dragPreviewForLiftingItem item: UIDragItem,
    session: any UIDragSession
) -> UITargetedDragPreview?
```

## Parameters 

`textDraggableView`  

The text view where the drag activity was started.

`item`  

The drag item that is being lifted.

`session`  

The drag session of the current drag activity.

## Return Value

A targeted drag preview to show during the lift animation, or `nil` to show the default preview.

## Discussion

You implement this method when you want to show a nondefault preview during the lift animation. If you return `nil`, the system shows default preview.

Note

This method is not called when the suggestedItems array for the text drag request contains the drag item.

