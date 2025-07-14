

- UIKit
- UICollectionViewFocusUpdateContext
-  nextFocusedIndexPath 

Instance Property

# nextFocusedIndexPath

The index path of the collection view cell that’s receiving the focus.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
var nextFocusedIndexPath: IndexPath? { get }
```

## Discussion

This property contains the index path only when the view receiving focus belongs to a cell of the collection view. If focus is moving to a view outside of the collection view and its cells, this property is `nil`.

## See Also

### Locating focusable items in the collection view

var previouslyFocusedIndexPath: IndexPath?

The index path of the collection view cell that previously had the focus.

