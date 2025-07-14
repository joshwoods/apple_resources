

- AppKit
- NSCollectionViewUpdateItem
-  indexPathAfterUpdate 

Instance Property

# indexPathAfterUpdate

The index path of the item after the update.

macOS 10.11+

``` source
@MainActor
var indexPathAfterUpdate: IndexPath? { get }
```

## Discussion

The value of this property is `nil` for an action of type NSCollectionView.UpdateAction.delete.

## See Also

### Accessing the Item Changes

var indexPathBeforeUpdate: IndexPath?

The index path of the item before the update.

var updateAction: NSCollectionView.UpdateAction

The action being performed on the item.

enum UpdateAction

Constants indicating the type of action being performed on an item.

enum ScrollDirection

Constants indicating the scrolling direction for the layout.

