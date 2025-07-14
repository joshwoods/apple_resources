

- AppKit
- NSTableView
-  NSTableView.DraggingDestinationFeedbackStyle 

Enumeration

# NSTableView.DraggingDestinationFeedbackStyle

These constants specify the drag styles displayed by the table view. They’re used by draggingDestinationFeedbackStyle.

macOS 10.6+

``` source
enum DraggingDestinationFeedbackStyle
```

## Topics

### Constants

case none

Provides no feedback when the user drags over the table view. This option exists to allow subclasses to implement their dragging destination highlighting, or to make it not show anything all.

case regular

Draws a solid round-rect background on drop target rows, and an insertion marker between rows. This style should be used in most cases.

case sourceList

Draws an outline on drop target rows, and an insertion marker between rows. This style will automatically be set for source lists when the table’s unhideRows(at:withAnimation:) is set to NSTableView.DraggingDestinationFeedbackStyle.sourceList. This is the standard look for Source Lists, but may be used in other areas as needed.

case gap

Provides a gap insertion when dragging over the table. Note that this style is only officially supported for NSView-based table views, but may partially work in Cell Based TableViews. The decision to use the gap style (compared to another style) can be made in tableView(_:draggingSession:willBeginAt:forRowIndexes:), or it can dynamically be changed.

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

enum RowSizeStyle

The row size style constants define the size of the rows in the table view. They are used by the effectiveRowSizeStyle and rowSizeStyle properties. You can also query the row size in the NSTableCellView class’ property rowSizeStyle.

enum RowActionEdge

These constants define table row edges on which row actions are attached. They are used by the `tableView:rowActionsForRow:edge:` delegate method.

