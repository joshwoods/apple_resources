

- UIKit
- UICollectionViewUpdateItem
-  UICollectionViewUpdateItem.Action 

Enumeration

# UICollectionViewUpdateItem.Action

Constants indicating the type of action being performed on an item.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
enum Action
```

## Topics

### Constants

case none

case insert

case delete

case reload

case move

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Accessing the item changes

var indexPathBeforeUpdate: IndexPath?

The index path of the item before the update.

var indexPathAfterUpdate: IndexPath?

The index path of the item after the update.

var updateAction: UICollectionViewUpdateItem.Action

The action being performed on the item.

