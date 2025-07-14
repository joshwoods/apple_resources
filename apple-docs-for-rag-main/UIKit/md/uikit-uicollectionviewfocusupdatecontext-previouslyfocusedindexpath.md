

- UIKit
- UICollectionViewFocusUpdateContext
-  previouslyFocusedIndexPath 

Instance Property

# previouslyFocusedIndexPath

The index path of the collection view cell that previously had the focus.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
var previouslyFocusedIndexPath: IndexPath? { get }
```

## Discussion

This property contains an index path only when the view receiving focus belongs to a cell of the collection view. If focus was previously in a view outside of the collection view and its cells, this property is `nil`. This property is also `nil` when the collection view receives focus for the first time.

## See Also

### Locating focusable items in the collection view

var nextFocusedIndexPath: IndexPath?

The index path of the collection view cell that’s receiving the focus.

