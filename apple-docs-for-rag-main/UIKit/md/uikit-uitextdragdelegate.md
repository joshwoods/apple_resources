

- UIKit
-  UITextDragDelegate 

Protocol

# UITextDragDelegate

The interface for customizing the behavior of a drag activity for a text view.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
protocol UITextDragDelegate : NSObjectProtocol
```

## Topics

### Handling drag session notifications

func textDraggableView(any UIView &amp; UITextDraggable, dragSessionWillBegin: any UIDragSession)

Tells the delegate that the text has been lifted out of the text view and the user is beginning to drag the text.

func textDraggableView(any UIView &amp; UITextDraggable, dragSessionDidEnd: any UIDragSession, with: UIDropOperation)

Tells the delegate that the drag session has ended.

### Providing additional animations

func textDraggableView(any UIView &amp; UITextDraggable, willAnimateLiftWith: any UIDragAnimating, session: any UIDragSession)

Tells the delegate when the lift animation is about to begin, and gives you a chance to animate additional changes alongside the system animation.

### Providing custom drag items

func textDraggableView(any UIView &amp; UITextDraggable, itemsForDrag: any UITextDragRequest) -> [UIDragItem]

Asks the delegate for custom drag items from a text view.

### Providing a custom preview for a drag activity

func textDraggableView(any UIView &amp; UITextDraggable, dragPreviewForLiftingItem: UIDragItem, session: any UIDragSession) -> UITargetedDragPreview?

Asks the delegate for the preview to show during the lift animation that happens when a user begins to drag an item from a text view.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Text view additions

protocol UITextDropDelegate

The interface for configuring a text view’s drop behavior.

protocol UITextDraggable

The interface that determines if a text view is a drag source.

struct UITextDragOptions

A set of options that determine the behavior of a draggable text view.

protocol UITextDroppable

The interface that determines if a text view is a drop destination.

enum UITextDropEditability

The text-drop editability styles for noneditable text views.

