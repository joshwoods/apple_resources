

- UIKit
- UICollectionViewUpdateItem
-  indexPathAfterUpdate 

Instance Property

# indexPathAfterUpdate

The index path of the item after the update.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var indexPathAfterUpdate: IndexPath? { get }
```

## See Also

### Accessing the item changes

var indexPathBeforeUpdate: IndexPath?

The index path of the item before the update.

var updateAction: UICollectionViewUpdateItem.Action

The action being performed on the item.

enum Action

Constants indicating the type of action being performed on an item.

