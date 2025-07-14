

- AppKit
- NSSplitViewDelegate
-  splitView(\_:shouldAdjustSizeOfSubview:) 

Instance Method

# splitView(\_:shouldAdjustSizeOfSubview:)

Allows the delegate to specify whether to resize the subview.

macOS 10.6+

``` source
@MainActor
optional func splitView(
    _ splitView: NSSplitView,
    shouldAdjustSizeOfSubview view: NSView
) -> Bool
```

## Parameters 

`splitView`  

The split view that sends the message.

`view`  

The subview to resize.

## Return Value

If adjustSubviews() can change the size of the subview, true; otherwise, false. By returning false, you lock the size of the split view `subview` while the split view resizes.

## Discussion

Important

If your split view uses Auto Layout to size its subviews, don’t implement this method.

Regardless of the value that this method returns, adjustSubviews() may change the origin of the subview. Nonresizable subviews may resize to prevent an invalid subview layout.

If a split view has no delegate, or if its delegate doesn’t respond to this message, the split view behaves as if this method returns true.

## See Also

### Adjusting Subviews Manually

func splitView(NSSplitView, constrainMinCoordinate: CGFloat, ofSubviewAt: Int) -> CGFloat

Allows the delegate to constrain the minimum coordinate limit of a divider when the user drags it.

func splitView(NSSplitView, constrainMaxCoordinate: CGFloat, ofSubviewAt: Int) -> CGFloat

Allows the delegate to constrain the maximum coordinate limit of a divider when the user drags it.

func splitView(NSSplitView, resizeSubviewsWithOldSize: NSSize)

Allows the delegate to specify custom sizing behavior for the subviews of the split view.

