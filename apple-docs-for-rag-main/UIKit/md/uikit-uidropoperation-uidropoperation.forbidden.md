

- UIKit
- UIDropOperation
-  UIDropOperation.forbidden 

Case

# UIDropOperation.forbidden

A drop operation type specifying that, although a move or copy operation is typically legitimate in this scenario, the drop activity isn’t allowed.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
case forbidden
```

## Discussion

You use this operation to signal that the drop activity isn’t allowed at this specific time and place. The drag operation is canceled.

## See Also

### Drop operation types

case cancel

A drop operation type specifying that no data should be transferred, thereby canceling the drag.

case copy

A drop operation type specifying that the data represented by the drag items should be copied to the destination view.

case move

A drop operation type specifying that the data represented by the drag items should be moved, not copied.

