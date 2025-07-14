

- UIKit
- UIDropOperation
-  UIDropOperation.move 

Case

# UIDropOperation.move

A drop operation type specifying that the data represented by the drag items should be moved, not copied.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
case move
```

## Discussion

You may use this operation only if the drop session’s allowsMoveOperation property is true; otherwise, it’s treated as a UIDropOperation.cancel operation. A move operation is allowed only within same app. Data shared with another app must be copied.

The system gives no special meaning to this operation. The UIDragInteractionDelegate object and the UIDropInteractionDelegate object must cooperate to produce the correct move results. For instance, the drop interaction delegate might insert the data in a new location while the drag interaction delegate removes the data from the old location.

## See Also

### Drop operation types

case cancel

A drop operation type specifying that no data should be transferred, thereby canceling the drag.

case forbidden

A drop operation type specifying that, although a move or copy operation is typically legitimate in this scenario, the drop activity isn’t allowed.

case copy

A drop operation type specifying that the data represented by the drag items should be copied to the destination view.

