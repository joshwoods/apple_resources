

- AppKit
- NSCollectionView
-  NSCollectionView.UpdateAction 

Enumeration

# NSCollectionView.UpdateAction

Constants indicating the type of action being performed on an item.

macOS 10.11+

``` source
enum UpdateAction
```

## Topics

### Constants

case insert

Insert the item into the collection view.

case delete

Remove the action from the collection view.

case reload

Reload the item, which consists of deleting and then inserting the item.

case move

Move the item from its current location to a new location.

case none

Take no action on the item.

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

### Enumerations

enum ScrollDirection

Constants indicating the scrolling direction for the layout.

