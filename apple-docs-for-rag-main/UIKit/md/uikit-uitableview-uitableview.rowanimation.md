

- UIKit
- UITableView
-  UITableView.RowAnimation 

Enumeration

# UITableView.RowAnimation

The type of animation to use when inserting or deleting rows.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
enum RowAnimation
```

## Overview

You specify one of these constants as a parameter of the insertRows(at:with:), insertSections(_:with:), deleteRows(at:with:),deleteSections(_:with:), reloadRows(at:with:), and reloadSections(_:with:) methods.

## Topics

### Constants

case fade

The inserted or deleted row or rows fade into or out of the table view.

case right

The inserted row or rows slide in from the right; the deleted row or rows slide out to the right.

case left

The inserted row or rows slide in from the left; the deleted row or rows slide out to the left.

case top

The inserted row or rows slide in from the top; the deleted row or rows slide out toward the top.

case bottom

The inserted row or rows slide in from the bottom; the deleted row or rows slide out toward the bottom.

case none

The inserted or deleted rows use the default animations.

case middle

The table view attempts to keep the old and new cells centered in the space they did or will occupy.

case automatic

The table view chooses an appropriate animation style for you.

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

### Inserting, deleting, and moving rows and sections

func insertRows(at: [IndexPath], with: UITableView.RowAnimation)

Inserts rows in the table view at the locations that an array of index paths identifies, with an option to animate the insertion.

func deleteRows(at: [IndexPath], with: UITableView.RowAnimation)

Deletes the rows that an array of index paths identifies, with an option to animate the deletion.

func insertSections(IndexSet, with: UITableView.RowAnimation)

Inserts one or more sections in the table view, with an option to animate the insertion.

func deleteSections(IndexSet, with: UITableView.RowAnimation)

Deletes one or more sections in the table view, with an option to animate the deletion.

func moveRow(at: IndexPath, to: IndexPath)

Moves the row at a specified location to a destination location.

func moveSection(Int, toSection: Int)

Moves a section to a new location in the table view.

