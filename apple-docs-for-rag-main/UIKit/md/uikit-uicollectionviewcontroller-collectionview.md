

- UIKit
- UICollectionViewController
-  collectionView 

Instance Property

# collectionView

The collection view object managed by this view controller.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var collectionView: UICollectionView! { get set }
```

## Discussion

If you assign a new collection view object to this property and that view’s data source or delegate aren’t yet set, the collection view controller makes itself the delegate or data source or both.

## See Also

### Getting the collection view

var collectionViewLayout: UICollectionViewLayout

The layout object used to initialize the collection view controller.

