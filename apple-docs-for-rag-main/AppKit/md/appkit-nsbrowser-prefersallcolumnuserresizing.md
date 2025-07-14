

- AppKit
- NSBrowser
-  prefersAllColumnUserResizing 

Instance Property

# prefersAllColumnUserResizing

A Boolean that indicates whether the browser is set to resize all columns simultaneously rather than resizing a single column at a time.

macOS

``` source
@MainActor
var prefersAllColumnUserResizing: Bool { get set }
```

## Discussion

When the value of this property is true, the browser is set to resize all columns simultaneously. The default value of this property is false.

This setting applies only to browsers that allow the user to resize columns (see the constant NSBrowser.ColumnResizingType.userColumnResizing). Holding down the Option key while resizing switches the type of resizing used. This setting is persistent.

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

