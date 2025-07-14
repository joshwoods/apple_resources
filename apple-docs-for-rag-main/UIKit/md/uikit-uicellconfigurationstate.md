

- UIKit
-  UICellConfigurationState 

Structure

# UICellConfigurationState

A structure that encapsulates a cell’s state.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
struct UICellConfigurationState
```

## Overview

A cell configuration state encompasses a trait collection along with all of the common states that affect a cell’s appearance — view states like selected, focused, or disabled, and cell states like editing or swiped. A cell configuration state encapsulates the inputs that configure a cell for any possible state or combination of states. You use a cell configuration state with background and content configurations to obtain the default appearance for a specific state.

Typically, you don’t create a configuration state yourself. To obtain a configuration state, override the updateConfiguration(using:) method in your cell subclass and use the state parameter. Outside of this method, you can get a cell’s configuration state by using its configurationState property.

You can create your own custom states to add to a cell configuration state by defining a custom state key using UIConfigurationStateCustomKey.

## Topics

### Managing view configuration states

var isSelected: Bool

A Boolean value that indicates whether the cell is in a selected state.

var isHighlighted: Bool

A Boolean value that indicates whether the cell is in a highlighted state.

var isFocused: Bool

A Boolean value that indicates whether the cell is in a focused state.

var isDisabled: Bool

A Boolean value that indicates whether the cell is in a disabled state.

var isPinned: Bool

A Boolean value that indicates whether the view is in a pinned state.

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

enum DropState

Constants that describe the cell’s drop state.

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- CustomReflectable
- CustomStringConvertible
- Equatable
- Hashable
- UIConfigurationState

## See Also

### Configuration states

struct UIViewConfigurationState

A structure that encapsulates a view’s state.

protocol UIConfigurationState

The requirements for an object that encapsulates a view’s state.

struct UIConfigurationStateCustomKey

A key that defines a custom state for a view.

