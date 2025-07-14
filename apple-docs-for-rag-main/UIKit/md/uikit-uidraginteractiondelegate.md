

- UIKit
-  UIDragInteractionDelegate 

Protocol

# UIDragInteractionDelegate

The interface for configuring and controlling a drag interaction.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
protocol UIDragInteractionDelegate : NSObjectProtocol
```

## Mentioned in 

Making a view into a drag source

Understanding a drag item as a promise

## Topics

### Performing the drag

func dragInteraction(UIDragInteraction, itemsForBeginning: any UIDragSession) -> [UIDragItem]

Asks the delegate for the array of drag items for an impending drag interaction.

**Required**

func dragInteraction(UIDragInteraction, itemsForAddingTo: any UIDragSession, withTouchAt: CGPoint) -> [UIDragItem]

Asks the delegate for the drag items to add to an in-progress drag session, in response to a user gesture to add the items.

func dragInteraction(UIDragInteraction, sessionForAddingItems: [any UIDragSession], withTouchAt: CGPoint) -> (any UIDragSession)?

Asks the delegate which drag session to add drag items to when there is more than one in-progress session.

### Animating the drag behaviors

func dragInteraction(UIDragInteraction, willAnimateLiftWith: any UIDragAnimating, session: any UIDragSession)

Tells the delegate the system’s lift animation is about to start.

func dragInteraction(UIDragInteraction, item: UIDragItem, willAnimateCancelWith: any UIDragAnimating)

Tells the delegate the system’s cancellation animation is about to start.

### Monitoring drag progress

func dragInteraction(UIDragInteraction, sessionWillBegin: any UIDragSession)

Tells the delegate the lift animation has finished and the user is starting to move the items across the screen.

func dragInteraction(UIDragInteraction, session: any UIDragSession, willAdd: [UIDragItem], for: UIDragInteraction)

Tells the delegate an interaction is about to add items to a drag session.

func dragInteraction(UIDragInteraction, sessionDidMove: any UIDragSession)

Tells the delegate the user moved the drag items to a new location on the screen.

func dragInteraction(UIDragInteraction, session: any UIDragSession, willEndWith: UIDropOperation)

Tells the delegate the drag activity will end with the specified operation.

func dragInteraction(UIDragInteraction, session: any UIDragSession, didEndWith: UIDropOperation)

Tells the delegate the drag activity and its related animations have finished.

func dragInteraction(UIDragInteraction, sessionDidTransferItems: any UIDragSession)

Tells the delegate the destination view has received the data for the drag items.

### Providing drag previews

func dragInteraction(UIDragInteraction, previewForLifting: UIDragItem, session: any UIDragSession) -> UITargetedDragPreview?

Asks the delegate for the targeted drag item preview that will appear during the lift animation.

func dragInteraction(UIDragInteraction, previewForCancelling: UIDragItem, withDefault: UITargetedDragPreview) -> UITargetedDragPreview?

Asks the delegate for the targeted drag item preview to show during the cancellation animation.

func dragInteraction(UIDragInteraction, prefersFullSizePreviewsFor: any UIDragSession) -> Bool

Asks the delegate whether the preview should appear in its original size or a scaled size.

### Restricting the drag behavior

func dragInteraction(UIDragInteraction, sessionIsRestrictedToDraggingApplication: any UIDragSession) -> Bool

Asks the delegate whether the system should restrict the drag session to the app that started the session.

func dragInteraction(UIDragInteraction, sessionAllowsMoveOperation: any UIDragSession) -> Bool

Asks the delegate whether the session allows the move operation.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Drag and drop interactions

protocol UIDropInteractionDelegate

The interface for configuring and controlling a drop interaction.

class UIDragInteraction

An interaction to enable dragging of items from a view, employing a delegate to provide drag items and to respond to calls from the drag session.

class UIDropInteraction

An interaction to enable dropping of items onto a view, employing a delegate to instantiate objects and respond to calls from the drop session.

