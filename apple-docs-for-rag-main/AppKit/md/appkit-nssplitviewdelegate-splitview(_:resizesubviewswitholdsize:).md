

- AppKit
- NSSplitViewDelegate
-  splitView(\_:resizeSubviewsWithOldSize:) 

Instance Method

# splitView(\_:resizeSubviewsWithOldSize:)

Allows the delegate to specify custom sizing behavior for the subviews of the split view.

macOS

``` source
@MainActor
optional func splitView(
    _ splitView: NSSplitView,
    resizeSubviewsWithOldSize oldSize: NSSize
)
```

## Parameters 

`splitView`  

The split view that sends the message.

`oldSize`  

The size of the split view before the user resizes it.

## Discussion

Important

If your split view uses Auto Layout to size its subviews, don’t implement this method.

If the delegate implements this method, it receives this message after the split view resizes.

Resize the subviews so that the sum of the sizes of the subviews plus the sum of the thickness of the dividers equals the size of the new frame of the NSSplitView. You can get the thickness of a divider through the dividerThickness method.

If you implement this delegate method to resize subviews on your own, the NSSplitView doesn’t perform any error checking for you. However, you can invoke adjustSubviews() to perform the default sizing behavior.

## See Also

### Adjusting Subviews Manually

func splitView(NSSplitView, constrainMinCoordinate: CGFloat, ofSubviewAt: Int) -> CGFloat

Allows the delegate to constrain the minimum coordinate limit of a divider when the user drags it.

func splitView(NSSplitView, constrainMaxCoordinate: CGFloat, ofSubviewAt: Int) -> CGFloat

Allows the delegate to constrain the maximum coordinate limit of a divider when the user drags it.

func splitView(NSSplitView, shouldAdjustSizeOfSubview: NSView) -> Bool

Allows the delegate to specify whether to resize the subview.

