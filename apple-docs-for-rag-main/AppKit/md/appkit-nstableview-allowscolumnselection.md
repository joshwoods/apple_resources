

- AppKit
- NSTableView
-  allowsColumnSelection 

Instance Property

# allowsColumnSelection

A Boolean value indicating whether the table view allows the user to select columns by clicking their headers.

macOS

``` source
@MainActor
var allowsColumnSelection: Bool { get set }
```

## Discussion

The default is false, which prevents the user from selecting columns (if you create the table view in Interface Builder, the default value is true). You can select columns programmatically regardless of this setting.

## See Also

### Configuring Behavior

var allowsColumnReordering: Bool

A Boolean value indicating whether the table view allows the user to rearrange columns by dragging their headers.

var allowsColumnResizing: Bool

A Boolean value indicating whether the table view allows the user to resize columns by dragging between their headers.

var allowsMultipleSelection: Bool

A Boolean value indicating whether the table view allows the user to select more than one column or row at a time.

var allowsEmptySelection: Bool

A Boolean value indicating whether the table view allows the user to select zero columns or rows.

var usesAutomaticRowHeights: Bool

A Boolean value that indicates whether the table view uses autolayout to calculate the height of rows.

