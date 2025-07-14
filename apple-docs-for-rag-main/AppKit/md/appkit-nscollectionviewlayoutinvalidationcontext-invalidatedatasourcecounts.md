

- AppKit
- NSCollectionViewLayoutInvalidationContext
-  invalidateDataSourceCounts 

Instance Property

# invalidateDataSourceCounts

A Boolean that indicates whether the layout object should ask for new section and item counts.

macOS 10.11+

``` source
@MainActor
var invalidateDataSourceCounts: Bool { get }
```

## Discussion

The collection view sets this property in response to specific layout invalidation scenarios. For example, the collection view sets the property to true when you insert or delete items or call the collection view’s reloadData() method.

When this property is set to true, the layout object must query the data source for the new number of sections and items. IT should also update its layout based on the updated number of sections and items.

## See Also

### Invalidating the Collection View Data

var invalidateEverything: Bool

A Boolean that indicates whether all layout data should be marked as invalid.

