

- AppKit
- NSTableCellView
-  imageView 

Instance Property

# imageView

Image displayed by the cell.

macOS 10.7+

``` source
@IBOutlet @MainActor
unowned(unsafe) var imageView: NSImageView? { get set }
```

## Discussion

This property is typically configured when the row is created in the NSTableViewDataSource protocol method tableView(_:viewFor:row:).

## See Also

### Displayed Items

var textField: NSTextField?

Text displayed by the cell.

