

- UIKit
- UITextDropDelegate
-  textDroppableView(\_:dropSessionDidEnd:) 

Instance Method

# textDroppableView(\_:dropSessionDidEnd:)

Tells the delegate that the drop session has ended.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func textDroppableView(
    _ textDroppableView: any UIView & UITextDroppable,
    dropSessionDidEnd session: any UIDropSession
)
```

## Parameters 

`textDroppableView`  

The text view that received the drop activity.

`session`  

The drop session that has ended.

## Discussion

You implement this method if your delegate needs to do additional cleanup after the drop session has ended.

## See Also

### Handling drop session notifications

func textDroppableView(any UIView &amp; UITextDroppable, dropSessionDidEnter: any UIDropSession)

Tells the delegate that the user has moved the drag items into the coordinate system of the text view.

func textDroppableView(any UIView &amp; UITextDroppable, dropSessionDidExit: any UIDropSession)

Tells the delegate that the user has moved the drag items out of the text view’s coordinate system.

func textDroppableView(any UIView &amp; UITextDroppable, dropSessionDidUpdate: any UIDropSession)

Tells the delegate that the drop session has been updated.

