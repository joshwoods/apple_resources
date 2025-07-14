

- AppKit
- NSTableColumn
-  headerCell 

Instance Property

# headerCell

The cell used to draw the table column’s header.

macOS

``` source
@MainActor
var headerCell: NSTableHeaderCell { get set }
```

## Discussion

The value of this property must not be `nil`. It’s recommended that the value of this property be an instance or subclass of NSTableHeaderCell.

You can set the table column title using the title property.

## See Also

### Setting the Header

var title: String

The title of the table column’s header.

