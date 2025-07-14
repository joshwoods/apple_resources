

- AppKit
- NSTableCellView
-  textField 

Instance Property

# textField

Text displayed by the cell.

macOS 10.7+

``` source
@IBOutlet @MainActor
unowned(unsafe) var textField: NSTextField? { get set }
```

## Discussion

This property is typically configured when the row is created in the NSTableViewDelegate protocol method tableView(_:viewFor:row:).

## See Also

### Displayed Items

var imageView: NSImageView?

Image displayed by the cell.

