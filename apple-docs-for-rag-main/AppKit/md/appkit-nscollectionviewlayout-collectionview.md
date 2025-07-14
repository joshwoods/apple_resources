

- AppKit
- NSCollectionViewLayout
-  collectionView 

Instance Property

# collectionView

The collection view object currently using this layout.

macOS 10.11+

``` source
@MainActor
weak var collectionView: NSCollectionView? { get }
```

## Discussion

When you assign a layout object to a collection view, the collection view automatically updates this property.

