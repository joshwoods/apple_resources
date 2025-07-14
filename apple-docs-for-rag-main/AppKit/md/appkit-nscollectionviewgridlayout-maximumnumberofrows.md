

- AppKit
- NSCollectionViewGridLayout
-  maximumNumberOfRows 

Instance Property

# maximumNumberOfRows

The maximum number of rows to display in the collection view’s visible area.

macOS 10.11+

``` source
@MainActor
var maximumNumberOfRows: Int { get set }
```

## Discussion

Use this value to specify the maximum number of rows to display in the collection view at any given time. The grid layout object uses this value during layout to configure the position and spacing of items. The default value of this property is `0`, which means that there is no maximum number of rows.

## See Also

### Specifying the Grid Parameters

var maximumNumberOfColumns: Int

The maximum number of columns to display in the collection view’s visible area.

var minimumItemSize: NSSize

The smallest allowable size for an item’s view.

var maximumItemSize: NSSize

The largest allowable size for an item’s view.

