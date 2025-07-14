

- UIKit
- UICellConfigurationState
-  UICellConfigurationState.DragState 

Enumeration

# UICellConfigurationState.DragState

Constants that describe the cell’s drag state.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
enum DragState
```

## Topics

### Drag states

case none

The system hasn’t associated the cell with a drag session.

case lifting

A user interaction is lifting the cell, but it isn’t yet part of an active drag session.

case dragging

The cell is part of an active drag session.

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

enum DropState

Constants that describe the cell’s drop state.

