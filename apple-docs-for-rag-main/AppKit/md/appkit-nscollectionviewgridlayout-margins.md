

- AppKit
- NSCollectionViewGridLayout
-  margins 

Instance Property

# margins

The amount of empty space (in points) around the grid’s content.

macOS 10.11+

``` source
@MainActor
var margins: NSEdgeInsets { get set }
```

## Discussion

The default value of this property is `NSEdgeInsetsZero`. Changing this property to a new value invalidates the layout.

## See Also

### Specifying the Grid Layout Attributes

var minimumInteritemSpacing: CGFloat

The minimum spacing (in points) to use between items in the same row or column.

var minimumLineSpacing: CGFloat

The minimum spacing (in points) to use between rows or columns.

