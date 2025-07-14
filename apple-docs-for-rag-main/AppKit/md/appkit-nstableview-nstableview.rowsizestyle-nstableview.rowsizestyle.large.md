

- AppKit
- NSTableView
- NSTableView.RowSizeStyle
-  NSTableView.RowSizeStyle.large 

Case

# NSTableView.RowSizeStyle.large

The table will use a row height specified for a large table. It is required that the size be fully tested and supported if `NSTableViewRowSizeStyleCustom` is not used.

macOS 10.7+

``` source
case large
```

## See Also

### Constants

case `default`

The table will use the system default layout size: small, medium or large.

case custom

The table will use the rowHeight or invoke the delegate method tableView(_:heightOfRow:), if implemented. The cell layout is not changed.

case small

The table will use a row height specified for a small table. It is required that the size be fully tested and supported if `NSTableViewRowSizeStyleCustom` is not used.

case medium

The table will use a row height specified for a medium table. It is required that the size be fully tested and supported if `NSTableViewRowSizeStyleCustom` is not used.

