

- UIKit
- UITextDropDelegate
-  textDroppableView(\_:dropSessionDidUpdate:) 

Instance Method

# textDroppableView(\_:dropSessionDidUpdate:)

Tells the delegate that the drop session has been updated.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func textDroppableView(
    _ textDroppableView: any UIView & UITextDroppable,
    dropSessionDidUpdate session: any UIDropSession
)
```

## Parameters 

`textDroppableView`  

The text view that received the drop activity.

`session`  

The current drop session.

## Discussion

The system usually—but not always—calls this method before calling the textDroppableView(_:proposalForDrop:) method. However, it’s called frequently, so do only what is necessary in your implementation.

## See Also

### Handling drop session notifications

func textDroppableView(any UIView &amp; UITextDroppable, dropSessionDidEnter: any UIDropSession)

Tells the delegate that the user has moved the drag items into the coordinate system of the text view.

func textDroppableView(any UIView &amp; UITextDroppable, dropSessionDidExit: any UIDropSession)

Tells the delegate that the user has moved the drag items out of the text view’s coordinate system.

func textDroppableView(any UIView &amp; UITextDroppable, dropSessionDidEnd: any UIDropSession)

Tells the delegate that the drop session has ended.

