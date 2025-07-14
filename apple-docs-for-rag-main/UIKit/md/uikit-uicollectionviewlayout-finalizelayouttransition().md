

- UIKit
- UICollectionViewLayout
-  finalizeLayoutTransition() 

Instance Method

# finalizeLayoutTransition()

Tells the layout object to perform any final steps before the transition animations occur.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func finalizeLayoutTransition()
```

## Discussion

The collection view calls this method after it has gathered all of the layout attributes needed to perform a transition from one layout to another. You can use this method to clean up any data structures or caches created by your implementations of the prepareForTransition(from:) or prepareForTransition(to:) methods.

## See Also

### Transitioning between layouts

func prepareForTransition(from: UICollectionViewLayout)

Tells the layout object to prepare to be installed as the layout for the collection view.

func prepareForTransition(to: UICollectionViewLayout)

Tells the layout object that it is about to be removed as the layout for the collection view.

