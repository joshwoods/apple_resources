

- AppKit
- NSBrowser
-  columnWidth(forColumnContentWidth:) 

Instance Method

# columnWidth(forColumnContentWidth:)

Returns the column width for the width of the given column’s content.

macOS

``` source
@MainActor
func columnWidth(forColumnContentWidth columnContentWidth: CGFloat) -> CGFloat
```

## Parameters 

`columnContentWidth`  

The width of the column’s content (the width of the matrix in the column).

## Return Value

The width of the column (the width of the entire scrolling text view).

## Discussion

For example, to guarantee that 16 pixels of your browser cell are always visible, call:

```
[browser setMinColumnWidth: [browser columnWidthForColumnContentWidth:16]]
```

## See Also

### Sizing

class func removeSavedColumns(withAutosaveName: NSBrowser.ColumnsAutosaveName)

Removes the column configuration data stored under the given name from the application’s user defaults.

var columnsAutosaveName: NSBrowser.ColumnsAutosaveName

The name used to automatically save the browser’s column configuration.

typealias ColumnsAutosaveName

func columnContentWidth(forColumnWidth: CGFloat) -> CGFloat

Returns the content width for a given column width.

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

