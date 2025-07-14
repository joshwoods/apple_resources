

- AppKit
- NSBrowser
-  columnContentWidth(forColumnWidth:) 

Instance Method

# columnContentWidth(forColumnWidth:)

Returns the content width for a given column width.

macOS

``` source
@MainActor
func columnContentWidth(forColumnWidth columnWidth: CGFloat) -> CGFloat
```

## Parameters 

`columnWidth`  

The width of the column. This width is the entire scrolling text view.

## Return Value

The width of the content for the column. This is the width of the matrix in the column.

## See Also

### Sizing

class func removeSavedColumns(withAutosaveName: NSBrowser.ColumnsAutosaveName)

Removes the column configuration data stored under the given name from the application’s user defaults.

var columnsAutosaveName: NSBrowser.ColumnsAutosaveName

The name used to automatically save the browser’s column configuration.

typealias ColumnsAutosaveName

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

var rowHeight: CGFloat

The height of the browser’s rows.

