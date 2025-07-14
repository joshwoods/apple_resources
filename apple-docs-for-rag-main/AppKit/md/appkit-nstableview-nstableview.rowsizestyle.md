

- AppKit
- NSTableView
-  NSTableView.RowSizeStyle 

Enumeration

# NSTableView.RowSizeStyle

The row size style constants define the size of the rows in the table view. They are used by the effectiveRowSizeStyle and rowSizeStyle properties. You can also query the row size in the NSTableCellView class’ property rowSizeStyle.

macOS 10.7+

``` source
enum RowSizeStyle
```

## Topics

### Constants

case `default`

The table will use the system default layout size: small, medium or large.

case custom

The table will use the rowHeight or invoke the delegate method tableView(_:heightOfRow:), if implemented. The cell layout is not changed.

case small

The table will use a row height specified for a small table. It is required that the size be fully tested and supported if `NSTableViewRowSizeStyleCustom` is not used.

case medium

The table will use a row height specified for a medium table. It is required that the size be fully tested and supported if `NSTableViewRowSizeStyleCustom` is not used.

case large

The table will use a row height specified for a large table. It is required that the size be fully tested and supported if `NSTableViewRowSizeStyleCustom` is not used.

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

### Constants

Specifying a Custom Row View in a Nib File

View-based table view instances use `NSTableViewRowKey` to identify the nib file containing the template row view. You can specify a custom row view (without any code) by associating this key with the appropriate nib name in Interface Builder.

enum DraggingDestinationFeedbackStyle

These constants specify the drag styles displayed by the table view. They’re used by draggingDestinationFeedbackStyle.

enum DropOperation

`NSTableView` defines these constants to specify drop operations.

struct GridLineStyle

`NSTableView` defines these constants to specify grid styles. These constants are used by the gridStyleMask property. The mask can be either NSTableViewGridNone or it can contain either or both of the other options combined using the C bitwise `OR` operator.

enum ColumnAutoresizingStyle

The following constants specify the autoresizing styles. These constants are used by the columnAutoresizingStyle property.

enum SelectionHighlightStyle

The following constants specify the selection highlight styles. These constants are used by the selectionHighlightStyle property.

struct AnimationOptions

Specifies the animation effects to apply when inserting or removing rows.

enum RowActionEdge

These constants define table row edges on which row actions are attached. They are used by the `tableView:rowActionsForRow:edge:` delegate method.

