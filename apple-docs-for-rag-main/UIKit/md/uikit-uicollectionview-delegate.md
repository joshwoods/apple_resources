

- UIKit
- UICollectionView
-  delegate 

Instance Property

# delegate

The object that acts as the delegate of the collection view.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
weak var delegate: (any UICollectionViewDelegate)? { get set }
```

## Discussion

The delegate must adopt the UICollectionViewDelegate protocol. The delegate object is responsible for managing selection behavior and interactions with individual items.

## See Also

### Managing collection view interactions

protocol UICollectionViewDelegate

The methods adopted by the object you use to manage user interactions with items in a collection view.

