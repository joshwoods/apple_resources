

- UIKit
- UICollectionView
-  visibleCells 

Instance Property

# visibleCells

An array of visible cells currently displayed by the collection view.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var visibleCells: [UICollectionViewCell] { get }
```

## Return Value

An array of UICollectionViewCell objects. If no cells are visible, this method returns an empty array.

## Discussion

This method returns the complete list of visible cells displayed by the collection view.

## See Also

### Related Documentation

var indexPathsForVisibleItems: [IndexPath]

An array of the visible items in the collection view.

### Getting the state of the collection view

var numberOfSections: Int

The number of sections displayed by the collection view.

func numberOfItems(inSection: Int) -> Int

Fetches the count of items in the specified section.

