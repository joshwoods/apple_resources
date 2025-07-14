

- UIKit
- UICollectionViewLayoutInvalidationContext
-  invalidateEverything 

Instance Property

# invalidateEverything

A Boolean that indicates that all layout data should be marked as invalid.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var invalidateEverything: Bool { get }
```

## Discussion

You do not set this property yourself. The collection view sets it in response to specific types of layout invalidation scenarios. For example, the collection view sets it to true when you change the current layout object, change the data source of the collection view, or call the reloadData() method and subsequently request a layout invalidation context.

If this property is set to true, the layout object should recompute all of its layout-related data.

## See Also

### Invalidating the Collection View Data

var invalidateDataSourceCounts: Bool

A Boolean that indicates whether the layout should ask for new section and item counts.

