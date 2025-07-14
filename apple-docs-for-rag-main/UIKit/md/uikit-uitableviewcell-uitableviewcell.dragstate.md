

- UIKit
- UITableViewCell
-  UITableViewCell.DragState 

Enumeration

# UITableViewCell.DragState

Constants indicating the current state of a row involved in a drag operation.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
enum DragState
```

## Topics

### Constants

case none

The cell isn’t involved in a drag operation.

case lifting

The cell is being animated off of the table’s surface.

case dragging

The cell is currently being dragged.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Dragging the row

var userInteractionEnabledWhileDragging: Bool

A Boolean value indicating whether users can interact with a cell while it is being dragged.

func dragStateDidChange(UITableViewCell.DragState)

Notifies the cell that its drag status changed.

