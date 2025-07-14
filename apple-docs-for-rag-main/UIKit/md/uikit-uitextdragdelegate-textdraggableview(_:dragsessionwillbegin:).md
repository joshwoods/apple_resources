

- UIKit
- UITextDragDelegate
-  textDraggableView(\_:dragSessionWillBegin:) 

Instance Method

# textDraggableView(\_:dragSessionWillBegin:)

Tells the delegate that the text has been lifted out of the text view and the user is beginning to drag the text.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func textDraggableView(
    _ textDraggableView: any UIView & UITextDraggable,
    dragSessionWillBegin session: any UIDragSession
)
```

## Parameters 

`textDraggableView`  

The text view where the drag activity was started.

`session`  

The drag session of the current drag activity.

## See Also

### Handling drag session notifications

func textDraggableView(any UIView &amp; UITextDraggable, dragSessionDidEnd: any UIDragSession, with: UIDropOperation)

Tells the delegate that the drag session has ended.

