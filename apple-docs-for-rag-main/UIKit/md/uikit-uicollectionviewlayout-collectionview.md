

- UIKit
- UICollectionViewLayout
-  collectionView 

Instance Property

# collectionView

The collection view object currently using this layout object.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var collectionView: UICollectionView? { get }
```

## Discussion

The collection view object sets the value of this property when a new layout object is assigned to it.

## See Also

### Getting the collection view information

var collectionViewContentSize: CGSize

The width and height of the collection view’s contents.

