

- AppKit
- NSTableRowView
-  backgroundColor 

Instance Property

# backgroundColor

The background color of the row.

macOS 10.7+

``` source
@NSCopying @MainActor
var backgroundColor: NSColor { get set }
```

## Discussion

The property defaults to the table view’s backgroundColor, unless usesAlternatingRowBackgroundColors is set to true. In that case, the colors alternate, and are automatically updated as required by insertions and deletions.

The value of the background color can be customized in the `NSTableViewDelegate` method `tableView:didAddRowView:forRow:`. The property is animatable.

## See Also

### Overriding Row View Display Characteristics

func drawBackground(in: NSRect)

Draws the background of the row in the rectangle.

func drawDraggingDestinationFeedback(in: NSRect)

Draws the row’s dragging destination feedback when the entire row is a drop target.

func drawSelection(in: NSRect)

Draws the selected row.

func drawSeparator(in: NSRect)

Draws the horizontal separator between table rows.

