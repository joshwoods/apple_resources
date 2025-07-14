

- AppKit
- NSCollectionViewGridLayout
-  maximumItemSize 

Instance Property

# maximumItemSize

The largest allowable size for an item’s view.

macOS 10.11+

``` source
@MainActor
var maximumItemSize: NSSize { get set }
```

## Discussion

Use this property to limit the maximum size of items displayed in the grid. The default value of this property is (`0.0`, `0.0`), which imposes no maximum size for items.

## See Also

### Specifying the Grid Parameters

var maximumNumberOfRows: Int

The maximum number of rows to display in the collection view’s visible area.

var maximumNumberOfColumns: Int

The maximum number of columns to display in the collection view’s visible area.

var minimumItemSize: NSSize

The smallest allowable size for an item’s view.

