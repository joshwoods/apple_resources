

- UIKit
- UITextDropDelegate
-  textDroppableView(\_:dropSessionDidExit:) 

Instance Method

# textDroppableView(\_:dropSessionDidExit:)

Tells the delegate that the user has moved the drag items out of the text view’s coordinate system.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func textDroppableView(
    _ textDroppableView: any UIView & UITextDroppable,
    dropSessionDidExit session: any UIDropSession
)
```

## Parameters 

`textDroppableView`  

The text view that received the drop activity.

`session`  

The current drop session.

## See Also

### Handling drop session notifications

func textDroppableView(any UIView &amp; UITextDroppable, dropSessionDidEnter: any UIDropSession)

Tells the delegate that the user has moved the drag items into the coordinate system of the text view.

func textDroppableView(any UIView &amp; UITextDroppable, dropSessionDidUpdate: any UIDropSession)

Tells the delegate that the drop session has been updated.

func textDroppableView(any UIView &amp; UITextDroppable, dropSessionDidEnd: any UIDropSession)

Tells the delegate that the drop session has ended.

