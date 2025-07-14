

- UIKit
- UICellConfigurationState
-  UICellConfigurationState.DropState 

Enumeration

# UICellConfigurationState.DropState

Constants that describe the cell’s drop state.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
enum DropState
```

## Topics

### Drop states

case none

The system hasn’t associated the cell with a drag session.

case notTargeted

A drag session is active and can perform a drop in the cell’s container, but the cell itself isn’t the drop target.

case targeted

The cell is the drop target for a drag session.

## Relationships

### Conforms To

- Equatable
- Hashable

## See Also

### Managing cell configuration states

var isEditing: Bool

A Boolean value that indicates whether the cell is in editing mode.

var isSwiped: Bool

A Boolean value that indicates whether the cell is in a swiped state.

var isExpanded: Bool

A Boolean value that indicates whether the cell is in an expanded state, such as in an outline.

var isReordering: Bool

A Boolean value that indicates whether the cell is reordering.

var cellDragState: UICellConfigurationState.DragState

The cell’s drag state.

var cellDropState: UICellConfigurationState.DropState

The cell’s drop state.

enum DragState

Constants that describe the cell’s drag state.

