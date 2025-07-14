

- AppKit
- NSTableView
-  NSTableView.DropOperation 

Enumeration

# NSTableView.DropOperation

`NSTableView` defines these constants to specify drop operations.

macOS

``` source
enum DropOperation
```

## Overview

For example, given a table with `n` rows (numbered with row `0` at the top visually), a row of `n–1` and operation of `NSTableViewDropOn` would specify a drop on the last row. To specify a drop below the last row, you use a row of `n` and `NSTableViewDropAbove` for the operation.

## Topics

### Constants

case on

Specifies that the drop should occur on the specified row.

case above

Specifies that the drop should occur above the specified row.

case on

Specifies that the drop should occur on the specified row.

case above

Specifies that the drop should occur above the specified row.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Constants

Specifying a Custom Row View in a Nib File

View-based table view instances use `NSTableViewRowKey` to identify the nib file containing the template row view. You can specify a custom row view (without any code) by associating this key with the appropriate nib name in Interface Builder.

enum DraggingDestinationFeedbackStyle

These constants specify the drag styles displayed by the table view. They’re used by draggingDestinationFeedbackStyle.

struct GridLineStyle

`NSTableView` defines these constants to specify grid styles. These constants are used by the gridStyleMask property. The mask can be either NSTableViewGridNone or it can contain either or both of the other options combined using the C bitwise `OR` operator.

enum ColumnAutoresizingStyle

The following constants specify the autoresizing styles. These constants are used by the columnAutoresizingStyle property.

enum SelectionHighlightStyle

The following constants specify the selection highlight styles. These constants are used by the selectionHighlightStyle property.

struct AnimationOptions

Specifies the animation effects to apply when inserting or removing rows.

enum RowSizeStyle

The row size style constants define the size of the rows in the table view. They are used by the effectiveRowSizeStyle and rowSizeStyle properties. You can also query the row size in the NSTableCellView class’ property rowSizeStyle.

enum RowActionEdge

These constants define table row edges on which row actions are attached. They are used by the `tableView:rowActionsForRow:edge:` delegate method.

