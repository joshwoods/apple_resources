

- UIKit
- UICollectionViewController
-  collectionViewLayout 

Instance Property

# collectionViewLayout

The layout object used to initialize the collection view controller.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var collectionViewLayout: UICollectionViewLayout { get }
```

## Discussion

This property contains the layout object you passed to the init(collectionViewLayout:) method. The layout object in this property isn’t updated to reflect changes to the collection view itself. You can use this property to refer to the layout object you originally configured the collection view to use.

## See Also

### Getting the collection view

var collectionView: UICollectionView!

The collection view object managed by this view controller.

