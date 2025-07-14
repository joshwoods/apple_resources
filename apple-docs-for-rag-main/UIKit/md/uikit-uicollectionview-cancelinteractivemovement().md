

- UIKit
- UICollectionView
-  cancelInteractiveMovement() 

Instance Method

# cancelInteractiveMovement()

Ends interactive movement tracking and returns the target item to its original location.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
func cancelInteractiveMovement()
```

## Discussion

Call this method to cancel movement tracking and return the item to its original location. For example, when using a gesture recognizer to track interactions, call this method when the gesture is cancelled. Calling this method lets the collection view know to end the tracking process and return the item to its original location.

## See Also

### Reordering items interactively

func beginInteractiveMovementForItem(at: IndexPath) -> Bool

Initiates the interactive movement of the item at the specified index path.

func updateInteractiveMovementTargetPosition(CGPoint)

Updates the position of the item within the collection view’s bounds.

func endInteractiveMovement()

Ends interactive movement tracking and moves the target item to its new location.

