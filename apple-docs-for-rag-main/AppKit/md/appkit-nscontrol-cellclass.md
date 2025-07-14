

- AppKit
- NSControl
-  cellClass 

Type Property

# cellClass

Returns the type of cell used by the receiver.

macOS

``` source
@MainActor
class var cellClass: AnyClass? { get set }
```

## Return Value

The class of the cell used to manage the receiver’s contents, or `nil` if no cell class has been set for the receiver or its superclasses (up to NSControl).

## See Also

### Deprecated Properties

var cell: NSCell?

The receiver’s cell object.

