

- AppKit
- NSTableView
-  NSTableView.AnimationOptions 

Structure

# NSTableView.AnimationOptions

Specifies the animation effects to apply when inserting or removing rows.

macOS 10.7+

``` source
struct AnimationOptions
```

## Topics

### Constants

static var effectFade: NSTableView.AnimationOptions

Use a fade for row or column removal. The effect can be combined with any of the slide constants.

static var effectGap: NSTableView.AnimationOptions

Creates a gap for newly inserted rows. This is useful for drag and drop animations that animate to a newly opened gap and should be used in the delegate method tableView(_:acceptDrop:row:dropOperation:).

static var slideUp: NSTableView.AnimationOptions

Animates a row insertion or removal by sliding upward.

static var slideDown: NSTableView.AnimationOptions

Animates a row insertion or removal by sliding downward.

static var slideLeft: NSTableView.AnimationOptions

Animates a row insertion by sliding from the left. Animates a row removal by sliding towards the left.

static var slideRight: NSTableView.AnimationOptions

Animates a row insertion by sliding from the right. Animates a row removal by sliding towards the right.

### Initializers

init(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

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

enum RowSizeStyle

The row size style constants define the size of the rows in the table view. They are used by the effectiveRowSizeStyle and rowSizeStyle properties. You can also query the row size in the NSTableCellView class’ property rowSizeStyle.

enum RowActionEdge

These constants define table row edges on which row actions are attached. They are used by the `tableView:rowActionsForRow:edge:` delegate method.

