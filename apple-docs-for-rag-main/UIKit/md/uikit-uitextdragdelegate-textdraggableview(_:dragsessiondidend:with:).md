

- UIKit
- UITextDragDelegate
-  textDraggableView(\_:dragSessionDidEnd:with:) 

Instance Method

# textDraggableView(\_:dragSessionDidEnd:with:)

Tells the delegate that the drag session has ended.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func textDraggableView(
    _ textDraggableView: any UIView & UITextDraggable,
    dragSessionDidEnd session: any UIDragSession,
    with operation: UIDropOperation
)
```

## Parameters 

`textDraggableView`  

The text view where the drag activity was started.

`session`  

The drag session of the current drag activity.

`operation`  

The operation that occurred during the drop activity.

## See Also

### Handling drag session notifications

func textDraggableView(any UIView &amp; UITextDraggable, dragSessionWillBegin: any UIDragSession)

Tells the delegate that the text has been lifted out of the text view and the user is beginning to drag the text.

