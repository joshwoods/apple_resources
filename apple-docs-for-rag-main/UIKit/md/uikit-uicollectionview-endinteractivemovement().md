

- UIKit
- UICollectionView
-  endInteractiveMovement() 

Instance Method

# endInteractiveMovement()

Ends interactive movement tracking and moves the target item to its new location.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
func endInteractiveMovement()
```

## Discussion

Call this method upon the successful completion of movement tracking for a item. For example, when using a gesture recognizer to track user interactions, call this method upon the successful completion of the gesture. Calling this method lets the collection view know to end tracking and move the item to its new location permanently. The collection view responds by calling the collectionView(_:moveItemAt:to:) method of its data source to ensure that your data structures are updated.

## See Also

### Reordering items interactively

func beginInteractiveMovementForItem(at: IndexPath) -> Bool

Initiates the interactive movement of the item at the specified index path.

func updateInteractiveMovementTargetPosition(CGPoint)

Updates the position of the item within the collection view’s bounds.

func cancelInteractiveMovement()

Ends interactive movement tracking and returns the target item to its original location.

