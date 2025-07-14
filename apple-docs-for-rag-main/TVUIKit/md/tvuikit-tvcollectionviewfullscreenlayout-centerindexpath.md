

- TVUIKit
- TVCollectionViewFullScreenLayout
-  centerIndexPath 

Instance Property

# centerIndexPath

The index path of the currently centered item.

tvOS 13.0+

``` source
@MainActor
var centerIndexPath: IndexPath? { get }
```

## Discussion

The `centerIndexPath` property returns the index path of the cell currently centered on the screen. `TVUIKit` calculates the current index path using the current content offset of the collection view.

