

- UIKit
- UITableViewCell
-  UITableViewCell.EditingStyle 

Enumeration

# UITableViewCell.EditingStyle

The editing control used by a cell.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
enum EditingStyle
```

## Overview

Use these constants with the editingStyle property.

## Topics

### Constants

case none

The cell has no editing control.

case delete

The cell has the delete editing control; this control is a red circle enclosing a minus sign.

case insert

The cell has the insert editing control; this control is a green circle enclosing a plus sign.

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

### Editing the cell

var isEditing: Bool

A Boolean value that indicates whether the cell is in an editable state.

func setEditing(Bool, animated: Bool)

Toggles the cell into and out of editing mode.

var editingStyle: UITableViewCell.EditingStyle

The editing style of the cell.

var showingDeleteConfirmation: Bool

A Boolean value that indicates whether the cell is currently showing the delete-confirmation button.

var showsReorderControl: Bool

A Boolean value that determines whether the cell shows the reordering control.

