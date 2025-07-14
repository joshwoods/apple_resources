

- AppKit
- NSCell
-  image 

Instance Property

# image

The image displayed by the cell, if any.

macOS

``` source
@MainActor
var image: NSImage? { get set }
```

## Discussion

Setting the value of this property converts the cell to an image-type cell, if it is not one already. The value of this property is `nil` if the cell is not an image-type cell.

## See Also

### Related Documentation

var type: NSCell.CellType

The type of the cell.

