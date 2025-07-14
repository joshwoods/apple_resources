

- UIKit
- UICollectionViewLayoutInvalidationContext
-  invalidateDataSourceCounts 

Instance Property

# invalidateDataSourceCounts

A Boolean that indicates whether the layout should ask for new section and item counts.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var invalidateDataSourceCounts: Bool { get }
```

## Discussion

You do not set this property yourself. The collection view sets it in response to specific types of layout invalidation scenarios. For example, the collection view sets it to true when you insert or delete items or call the collection view’s reloadData() method.

If this property is set to true, the layout object should query its delegate for the number of sections and items and update its layout based on the new number of items.

## See Also

### Invalidating the Collection View Data

var invalidateEverything: Bool

A Boolean that indicates that all layout data should be marked as invalid.

