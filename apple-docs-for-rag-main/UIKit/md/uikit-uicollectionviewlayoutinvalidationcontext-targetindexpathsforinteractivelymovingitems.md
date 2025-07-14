

- UIKit
- UICollectionViewLayoutInvalidationContext
-  targetIndexPathsForInteractivelyMovingItems 

Instance Property

# targetIndexPathsForInteractivelyMovingItems

An array of index paths representing the new location of moving items in the collection view.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
var targetIndexPathsForInteractivelyMovingItems: [IndexPath]? { get }
```

## Discussion

This property is filled when an interactive move is in progress or has just ended. Use this property together with the previousIndexPathsForInteractivelyMovingItems property to determine what changes you need to make to the affected items. For most other updates, the value of this property is `nil`.

## See Also

### Invalidating the Order of Items

var previousIndexPathsForInteractivelyMovingItems: [IndexPath]?

An array of index paths representing the previous location of moving items in the collection view.

var interactiveMovementTarget: CGPoint

The current point used to determine the placement of moving items.

