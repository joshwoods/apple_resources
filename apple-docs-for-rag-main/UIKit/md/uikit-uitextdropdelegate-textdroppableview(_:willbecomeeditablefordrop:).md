

- UIKit
- UITextDropDelegate
-  textDroppableView(\_:willBecomeEditableForDrop:) 

Instance Method

# textDroppableView(\_:willBecomeEditableForDrop:)

Asks the delegate if a noneditable text view can accept a drop operation.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func textDroppableView(
    _ textDroppableView: any UIView & UITextDroppable,
    willBecomeEditableForDrop drop: any UITextDropRequest
) -> UITextDropEditability
```

## Parameters 

`textDroppableView`  

The text view that received the drop activity.

`drop`  

The drop request.

## Return Value

A text drop editability style that indicates whether the text view can accept a drop operation.

## Discussion

By default, a text view that is not editable can’t accept drop requests. However, you can change this behavior by returning the editability style UITextDropEditability.temporary or UITextDropEditability.yes in your implementation of this method. Not implementing this method is the same as returning the UITextDropEditability.no style.

## See Also

### Accepting a drop activity

func textDroppableView(any UIView &amp; UITextDroppable, proposalForDrop: any UITextDropRequest) -> UITextDropProposal

Asks the delegate if the text view can accept a drop operation.

