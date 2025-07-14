

- AppKit
- NSCollectionViewGridLayout
-  maximumNumberOfColumns 

Instance Property

# maximumNumberOfColumns

The maximum number of columns to display in the collection view’s visible area.

macOS 10.11+

``` source
@MainActor
var maximumNumberOfColumns: Int { get set }
```

## Discussion

Use this value to specify the maximum number of columns that should be visible in the collection view at any given time. The grid layout object uses this value during layout to configure the position and spacing of items. The default value of this property is `0`, which means that there is no maximum number of columns.

## See Also

### Specifying the Grid Parameters

var maximumNumberOfRows: Int

The maximum number of rows to display in the collection view’s visible area.

var minimumItemSize: NSSize

The smallest allowable size for an item’s view.

var maximumItemSize: NSSize

The largest allowable size for an item’s view.

