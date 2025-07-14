

- AppKit
- NSBrowser
-  setWidth(\_:ofColumn:) 

Instance Method

# setWidth(\_:ofColumn:)

Sets the width of the specified column.

macOS

``` source
@MainActor
func setWidth(
    _ columnWidth: CGFloat,
    ofColumn columnIndex: Int
)
```

## Parameters 

`columnWidth`  

The new width of the specified column.

`columnIndex`  

The index of the column for which to set the width.

## Discussion

This method can be used to set the initial width of browser columns unless the column sizing is automatic; setWidth(_:ofColumn:) does nothing if columnResizingType is NSBrowser.ColumnResizingType.autoColumnResizing. To set the default width for new columns (that don’t otherwise have initial widths from defaults or via the delegate), use a `columnIndex` of –1. A value set for `columnIndex` of –1 is persistent. An columnConfigurationDidChangeNotification notification is posted (not immediately), if necessary, so that the browser can autosave the new column configuration.

## See Also

### Related Documentation

func browser(NSBrowser, shouldSizeColumn: Int, forUserResize: Bool, toWidth: CGFloat) -> CGFloat

Used to determine a column’s initial size.

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

func defaultColumnWidth() -> CGFloat

Returns the default column width of the browser’s columns.

func setDefaultColumnWidth(CGFloat)

Sets the default column width for new browser columns that do not otherwise have an initial width from defaults or the browser’s delegate.

var rowHeight: CGFloat

The height of the browser’s rows.

