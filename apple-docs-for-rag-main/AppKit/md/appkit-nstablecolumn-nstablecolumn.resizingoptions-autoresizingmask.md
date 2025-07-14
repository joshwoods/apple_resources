

- AppKit
- NSTableColumn
- NSTableColumn.ResizingOptions
-  autoresizingMask 

Type Property

# autoresizingMask

Allows the table column to resize automatically in response to resizing the table view. The resizing behavior for the table view is set using the `NSTableView` method columnAutoresizingStyle.

macOS

``` source
static var autoresizingMask: NSTableColumn.ResizingOptions { get }
```

## See Also

### Constants

static var userResizingMask: NSTableColumn.ResizingOptions

Allows the table column to be resized by the user.

