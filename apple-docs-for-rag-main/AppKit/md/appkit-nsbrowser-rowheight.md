

- AppKit
- NSBrowser
-  rowHeight 

Instance Property

# rowHeight

The height of the browser’s rows.

macOS 10.6+

``` source
@MainActor
var rowHeight: CGFloat { get set }
```

## Discussion

The value of this property must be greater than `0`. The default value of this property is `17.0`. Any fractional value will be forced to an integral value for drawing. For variable row height browsers (ones whose delegates implement browser(_:heightOfRow:inColumn:)), the row height will be used to draw alternating rows past the last row in each browser column.

This property is only available when using the item delegate methods. An exception is thrown if you are using the matrix delegate methods.

## See Also

### Sizing

class func removeSavedColumns(withAutosaveName: NSBrowser.ColumnsAutosaveName)

Removes the column configuration data stored under the given name from the application’s user defaults.

var columnsAutosaveName: NSBrowser.ColumnsAutosaveName

The name used to automatically save the browser’s column configuration.

typealias ColumnsAutosaveName

func columnContentWidth(forColumnWidth: CGFloat) -> CGFloat

Returns the content width for a given column width.

func columnWidth(forColumnContentWidth: CGFloat) -> CGFloat

Returns the column width for the width of the given column’s content.

var columnResizingType: NSBrowser.ColumnResizingType

A constant indicating the browser’s column resizing type.

var prefersAllColumnUserResizing: Bool

A Boolean that indicates whether the browser is set to resize all columns simultaneously rather than resizing a single column at a time.

func width(ofColumn: Int) -> CGFloat

Returns the width of the specified column.

func setWidth(CGFloat, ofColumn: Int)

Sets the width of the specified column.

func defaultColumnWidth() -> CGFloat

Returns the default column width of the browser’s columns.

func setDefaultColumnWidth(CGFloat)

Sets the default column width for new browser columns that do not otherwise have an initial width from defaults or the browser’s delegate.

