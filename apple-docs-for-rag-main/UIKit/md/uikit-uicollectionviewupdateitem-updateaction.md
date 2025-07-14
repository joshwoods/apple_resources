

- UIKit
- UICollectionViewUpdateItem
-  updateAction 

Instance Property

# updateAction

The action being performed on the item.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var updateAction: UICollectionViewUpdateItem.Action { get }
```

## Discussion

For a list of relevant action types, see UICollectionViewUpdateItem.Action.

## See Also

### Accessing the item changes

var indexPathBeforeUpdate: IndexPath?

The index path of the item before the update.

var indexPathAfterUpdate: IndexPath?

The index path of the item after the update.

enum Action

Constants indicating the type of action being performed on an item.

