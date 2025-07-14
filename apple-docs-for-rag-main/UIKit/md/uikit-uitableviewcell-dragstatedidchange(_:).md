

- UIKit
- UITableViewCell
-  dragStateDidChange(\_:) 

Instance Method

# dragStateDidChange(\_:)

Notifies the cell that its drag status changed.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func dragStateDidChange(_ dragState: UITableViewCell.DragState)
```

## Parameters 

`dragState`  

The new drag state for the cell.

## See Also

### Dragging the row

var userInteractionEnabledWhileDragging: Bool

A Boolean value indicating whether users can interact with a cell while it is being dragged.

enum DragState

Constants indicating the current state of a row involved in a drag operation.

