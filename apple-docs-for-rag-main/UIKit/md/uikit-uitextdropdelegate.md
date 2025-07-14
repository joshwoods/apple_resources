

- UIKit
-  UITextDropDelegate 

Protocol

# UITextDropDelegate

The interface for configuring a text view’s drop behavior.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
protocol UITextDropDelegate : NSObjectProtocol
```

## Topics

### Accepting a drop activity

func textDroppableView(any UIView &amp; UITextDroppable, proposalForDrop: any UITextDropRequest) -> UITextDropProposal

Asks the delegate if the text view can accept a drop operation.

func textDroppableView(any UIView &amp; UITextDroppable, willBecomeEditableForDrop: any UITextDropRequest) -> UITextDropEditability

Asks the delegate if a noneditable text view can accept a drop operation.

### Handling drop session notifications

func textDroppableView(any UIView &amp; UITextDroppable, dropSessionDidEnter: any UIDropSession)

Tells the delegate that the user has moved the drag items into the coordinate system of the text view.

func textDroppableView(any UIView &amp; UITextDroppable, dropSessionDidExit: any UIDropSession)

Tells the delegate that the user has moved the drag items out of the text view’s coordinate system.

func textDroppableView(any UIView &amp; UITextDroppable, dropSessionDidUpdate: any UIDropSession)

Tells the delegate that the drop session has been updated.

func textDroppableView(any UIView &amp; UITextDroppable, dropSessionDidEnd: any UIDropSession)

Tells the delegate that the drop session has ended.

### Handling drop activity notifications

func textDroppableView(any UIView &amp; UITextDroppable, willPerformDrop: any UITextDropRequest)

Tells the delegate that the drop operation is about to happen.

### Providing a custom preview for a drop activity

func textDroppableView(any UIView &amp; UITextDroppable, previewForDroppingAllItemsWithDefault: UITargetedDragPreview) -> UITargetedDragPreview?

Asks the delegate for the preview to show during the drop animation.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Text view additions

protocol UITextDragDelegate

The interface for customizing the behavior of a drag activity for a text view.

protocol UITextDraggable

The interface that determines if a text view is a drag source.

struct UITextDragOptions

A set of options that determine the behavior of a draggable text view.

protocol UITextDroppable

The interface that determines if a text view is a drop destination.

enum UITextDropEditability

The text-drop editability styles for noneditable text views.

