

- UIKit
- UIDropInteractionDelegate
-  dropInteraction(\_:item:willAnimateDropWith:) 

Instance Method

# dropInteraction(\_:item:willAnimateDropWith:)

Tells the delegate the system’s drop animation is about to start.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func dropInteraction(
    _ interaction: UIDropInteraction,
    item: UIDragItem,
    willAnimateDropWith animator: any UIDragAnimating
)
```

## Parameters 

`interaction`  

The interaction that called this method.

`item`  

The current drag item.

`animator`  

The animator that provides custom animations to run alongside the system’s drop animation. You can also use it to add a completion block that runs after the animations have finished.

## Discussion

This method is called for each drag item in the session, whether the item’s visible or not.

## See Also

### Animating the drop

func dropInteraction(UIDropInteraction, previewForDropping: UIDragItem, withDefault: UITargetedDragPreview) -> UITargetedDragPreview?

Asks the delegate for the targeted drag item preview to show during the drop animation.

func dropInteraction(UIDropInteraction, concludeDrop: any UIDropSession)

Tells the delegate the drop activity and its related animations have finished.

