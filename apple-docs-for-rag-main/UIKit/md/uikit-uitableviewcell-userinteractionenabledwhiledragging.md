

- UIKit
- UITableViewCell
-  userInteractionEnabledWhileDragging 

Instance Property

# userInteractionEnabledWhileDragging

A Boolean value indicating whether users can interact with a cell while it is being dragged.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var userInteractionEnabledWhileDragging: Bool { get set }
```

## Discussion

The default value of this property is false.

## See Also

### Dragging the row

func dragStateDidChange(UITableViewCell.DragState)

Notifies the cell that its drag status changed.

enum DragState

Constants indicating the current state of a row involved in a drag operation.

