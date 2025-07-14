

- AppKit
- NSCollectionViewLayoutInvalidationContext
-  invalidateEverything 

Instance Property

# invalidateEverything

A Boolean that indicates whether all layout data should be marked as invalid.

macOS 10.11+

``` source
@MainActor
var invalidateEverything: Bool { get }
```

## Discussion

The collection view sets this property in response to specific layout invalidation scenarios. For example, the collection view sets the property to true when you change the current layout object, change the data source of the collection view, or call the reloadData() method and subsequently request a layout invalidation context.

When this property is set to true, the layout object must throw away all previous layout information and recompute it.

## See Also

### Invalidating the Collection View Data

var invalidateDataSourceCounts: Bool

A Boolean that indicates whether the layout object should ask for new section and item counts.

