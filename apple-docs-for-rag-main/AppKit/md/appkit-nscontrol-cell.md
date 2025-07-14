

- AppKit
- NSControl
-  cell 

Instance Property

# cell

The receiver’s cell object.

macOS

``` source
@MainActor
var cell: NSCell? { get set }
```

## Discussion

For controls with multiple cells (such as `NSMatrix` or `NSForm`), use the selectedCell() property to retrieve a specific cell.

## See Also

### Deprecated Properties

class var cellClass: AnyClass?

Returns the type of cell used by the receiver.

