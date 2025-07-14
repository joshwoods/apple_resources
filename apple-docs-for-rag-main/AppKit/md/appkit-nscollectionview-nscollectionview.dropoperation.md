

- AppKit
- NSCollectionView
-  NSCollectionView.DropOperation 

Enumeration

# NSCollectionView.DropOperation

These constants specify if acceptance of a drop should be at the item it is dropped on or before the item. These constants are used by the collectionView(_:acceptDrop:index:dropOperation:) and collectionView(_:validateDrop:proposedIndex:dropOperation:) methods in NSCollectionViewDelegate

macOS 10.6+

``` source
enum DropOperation
```

## Topics

### Constants

case on

The drop occurs at the collection view item to which the item was dragged.

case before

The drop occurs before the collection view item to which the item was dragged.

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

### Constants

struct ScrollPosition

Constants indicating the options for scrolling the collection view’s content.

