

- AppKit
- NSCollectionViewGridLayout
-  minimumItemSize 

Instance Property

# minimumItemSize

The smallest allowable size for an item’s view.

macOS 10.11+

``` source
@MainActor
var minimumItemSize: NSSize { get set }
```

## Discussion

Use this property to ensure that items have a minimum size when displayed in the grid. The default value of this property is (`0.0`, `0.0`), which imposes no minimum size for items.

## See Also

### Specifying the Grid Parameters

var maximumNumberOfRows: Int

The maximum number of rows to display in the collection view’s visible area.

var maximumNumberOfColumns: Int

The maximum number of columns to display in the collection view’s visible area.

var maximumItemSize: NSSize

The largest allowable size for an item’s view.

