

- UIKit
- UIDropInteractionDelegate
-  dropInteraction(\_:concludeDrop:) 

Instance Method

# dropInteraction(\_:concludeDrop:)

Tells the delegate the drop activity and its related animations have finished.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func dropInteraction(
    _ interaction: UIDropInteraction,
    concludeDrop session: any UIDropSession
)
```

## Parameters 

`interaction`  

The interaction that called this method.

`session`  

The drop session that has finished.

## Discussion

When the interaction calls this method, update the interaction’s view with its post-drop appearance.

## See Also

### Animating the drop

func dropInteraction(UIDropInteraction, item: UIDragItem, willAnimateDropWith: any UIDragAnimating)

Tells the delegate the system’s drop animation is about to start.

func dropInteraction(UIDropInteraction, previewForDropping: UIDragItem, withDefault: UITargetedDragPreview) -> UITargetedDragPreview?

Asks the delegate for the targeted drag item preview to show during the drop animation.

