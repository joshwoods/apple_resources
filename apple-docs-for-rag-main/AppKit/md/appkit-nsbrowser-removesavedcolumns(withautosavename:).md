

- AppKit
- NSBrowser
-  removeSavedColumns(withAutosaveName:) 

Type Method

# removeSavedColumns(withAutosaveName:)

Removes the column configuration data stored under the given name from the application’s user defaults.

macOS

``` source
@MainActor
class func removeSavedColumns(withAutosaveName name: NSBrowser.ColumnsAutosaveName)
```

## Parameters 

`name`  

The name of the column configuration data to remove.

## See Also

### Sizing

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

var rowHeight: CGFloat

The height of the browser’s rows.

