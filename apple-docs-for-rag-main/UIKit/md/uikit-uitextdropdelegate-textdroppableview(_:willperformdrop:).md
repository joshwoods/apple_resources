

- UIKit
- UITextDropDelegate
-  textDroppableView(\_:willPerformDrop:) 

Instance Method

# textDroppableView(\_:willPerformDrop:)

Tells the delegate that the drop operation is about to happen.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func textDroppableView(
    _ textDroppableView: any UIView & UITextDroppable,
    willPerformDrop drop: any UITextDropRequest
)
```

## Parameters 

`textDroppableView`  

The text view that received the drop activity.

`drop`  

The drop request.

## Discussion

If you need to modify the drag items before the drop operation happens, provide the text view a pasteDelegate object that implements the paste(itemProviders:) method. In the implementation, do the item conversion and paste the text.

