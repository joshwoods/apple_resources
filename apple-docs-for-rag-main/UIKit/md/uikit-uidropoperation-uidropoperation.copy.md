

- UIKit
- UIDropOperation
-  UIDropOperation.copy 

Case

# UIDropOperation.copy

A drop operation type specifying that the data represented by the drag items should be copied to the destination view.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
case copy
```

## Discussion

This operation is used most often. When the user performs a drop activity, the dropInteraction(_:performDrop:) delegate method is called. Your implementation of this delegate method should copy the data from the drag items to the destination view.

## See Also

### Drop operation types

case cancel

A drop operation type specifying that no data should be transferred, thereby canceling the drag.

case forbidden

A drop operation type specifying that, although a move or copy operation is typically legitimate in this scenario, the drop activity isn’t allowed.

case move

A drop operation type specifying that the data represented by the drag items should be moved, not copied.

