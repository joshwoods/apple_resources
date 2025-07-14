

- UIKit
-  UIDropInteractionDelegate 

Protocol

# UIDropInteractionDelegate

The interface for configuring and controlling a drop interaction.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
protocol UIDropInteractionDelegate : NSObjectProtocol
```

## Mentioned in 

Making a view into a drop destination

Understanding a drag item as a promise

## Topics

### Handling the drop

func dropInteraction(UIDropInteraction, canHandle: any UIDropSession) -> Bool

Asks the delegate whether it can handle the session’s drag items.

func dropInteraction(UIDropInteraction, performDrop: any UIDropSession)

Tells the delegate it can request the item provider data from the session’s drag items.

### Tracking the drop movements

func dropInteraction(UIDropInteraction, sessionDidEnter: any UIDropSession)

Tells the delegate the drop session has moved into the drop interaction’s view.

func dropInteraction(UIDropInteraction, sessionDidUpdate: any UIDropSession) -> UIDropProposal

Tells the delegate the drop session has changed.

func dropInteraction(UIDropInteraction, sessionDidExit: any UIDropSession)

Tells the delegate the drop session has moved out of the drop interaction’s view.

func dropInteraction(UIDropInteraction, sessionDidEnd: any UIDropSession)

Tells the delegate the drop session has ended.

### Animating the drop

func dropInteraction(UIDropInteraction, item: UIDragItem, willAnimateDropWith: any UIDragAnimating)

Tells the delegate the system’s drop animation is about to start.

func dropInteraction(UIDropInteraction, previewForDropping: UIDragItem, withDefault: UITargetedDragPreview) -> UITargetedDragPreview?

Asks the delegate for the targeted drag item preview to show during the drop animation.

func dropInteraction(UIDropInteraction, concludeDrop: any UIDropSession)

Tells the delegate the drop activity and its related animations have finished.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Drag and drop interactions

protocol UIDragInteractionDelegate

The interface for configuring and controlling a drag interaction.

class UIDragInteraction

An interaction to enable dragging of items from a view, employing a delegate to provide drag items and to respond to calls from the drag session.

class UIDropInteraction

An interaction to enable dropping of items onto a view, employing a delegate to instantiate objects and respond to calls from the drop session.

