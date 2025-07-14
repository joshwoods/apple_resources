

- UIKit
- UICollectionViewCell
-  dragStateDidChange(\_:) 

Instance Method

# dragStateDidChange(\_:)

Called when the drag state of the cell changes.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func dragStateDidChange(_ dragState: UICollectionViewCell.DragState)
```

## Discussion

Subclasses can override this method and use it to change the cell’s appearance during drag and drop operations. For example, you might use this method to hide or disable controls that you do not want to be visible while the cell is being dragged. You can also use this method to alter the disabled appearance of the cell that remains in the collection view at the original location of the drag.

## See Also

### Managing drag state changes

enum DragState

Constants indicating the current state of the drag operation.

