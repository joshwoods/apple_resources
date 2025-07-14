

- UIKit
- UICollectionViewCell
-  UICollectionViewCell.DragState 

Enumeration

# UICollectionViewCell.DragState

Constants indicating the current state of the drag operation.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
enum DragState
```

## Topics

### Constants

case none

The cell isn’t involved in a drag.

case lifting

The cell is being animated off of the surface of the collection view.

case dragging

The cell is being dragged.

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

### Managing drag state changes

func dragStateDidChange(UICollectionViewCell.DragState)

Called when the drag state of the cell changes.

