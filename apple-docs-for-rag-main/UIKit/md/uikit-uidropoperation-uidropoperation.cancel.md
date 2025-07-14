

- UIKit
- UIDropOperation
-  UIDropOperation.cancel 

Case

# UIDropOperation.cancel

A drop operation type specifying that no data should be transferred, thereby canceling the drag.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
case cancel
```

## Mentioned in 

Making a view into a drop destination

## Discussion

If the user attempts a drop activity, the drag operation is canceled and the dropInteraction(_:performDrop:) delegate method isn’t called.

## See Also

### Drop operation types

case forbidden

A drop operation type specifying that, although a move or copy operation is typically legitimate in this scenario, the drop activity isn’t allowed.

case copy

A drop operation type specifying that the data represented by the drag items should be copied to the destination view.

case move

A drop operation type specifying that the data represented by the drag items should be moved, not copied.

