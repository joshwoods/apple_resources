

- AppKit
- NSTableView
-  effectiveRowSizeStyle 

Instance Property

# effectiveRowSizeStyle

The effective row size style for the table.

macOS 10.7+

``` source
@MainActor
var effectiveRowSizeStyle: NSTableView.RowSizeStyle { get }
```

## Discussion

If the value in the rowSizeStyle property is NSTableView.RowSizeStyle.default, then this property contains the default size for this table. The default size is currently set in System Preferences by the user.

## See Also

### Getting and Setting Row Size Styles

var rowSizeStyle: NSTableView.RowSizeStyle

The row size style (small, medium, large, or custom) used by the table view.

