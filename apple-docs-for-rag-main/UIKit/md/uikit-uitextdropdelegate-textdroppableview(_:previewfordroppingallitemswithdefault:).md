

- UIKit
- UITextDropDelegate
-  textDroppableView(\_:previewForDroppingAllItemsWithDefault:) 

Instance Method

# textDroppableView(\_:previewForDroppingAllItemsWithDefault:)

Asks the delegate for the preview to show during the drop animation.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func textDroppableView(
    _ textDroppableView: any UIView & UITextDroppable,
    previewForDroppingAllItemsWithDefault defaultPreview: UITargetedDragPreview
) -> UITargetedDragPreview?
```

## Parameters 

`textDroppableView`  

The text view that received the drop activity.

`defaultPreview`  

The preview that is displayed when the delegate doesn’t provide this method.

## Return Value

A target drag preview to show during the drop animation, or `nil` to show the default preview.

## Discussion

You implement this method when you want to show a nondefault preview during the drop animation. If you return `nil`, the system shows the default preview.

