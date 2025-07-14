

- AppKit
- NSCollectionViewUpdateItem
-  updateAction 

Instance Property

# updateAction

The action being performed on the item.

macOS 10.11+

``` source
@MainActor
var updateAction: NSCollectionView.UpdateAction { get }
```

## Discussion

For a list of relevant actions, see NSCollectionView.UpdateAction.

## See Also

### Accessing the Item Changes

var indexPathBeforeUpdate: IndexPath?

The index path of the item before the update.

var indexPathAfterUpdate: IndexPath?

The index path of the item after the update.

enum UpdateAction

Constants indicating the type of action being performed on an item.

enum ScrollDirection

Constants indicating the scrolling direction for the layout.

