

- UIKit
- UICollectionView
-  UICollectionView.ReorderingCadence 

Enumeration

# UICollectionView.ReorderingCadence

Constants indicating the speed at which collection view items are reorganized during a drop.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
enum ReorderingCadence
```

## Topics

### Constants

case immediate

Items are reordered into place immediately.

case fast

Items are reordered quickly, but with a short delay.

case slow

Items are reordered after a delay.

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

### Managing drop interactions

var dropDelegate: (any UICollectionViewDropDelegate)?

The delegate object that manages the dropping of items into the collection view.

protocol UICollectionViewDropDelegate

The interface for handling drops in a collection view.

var hasActiveDrop: Bool

A Boolean value that indicates whether the collection view is currently tracking a drop session.

var reorderingCadence: UICollectionView.ReorderingCadence

The speed at which items in the collection view are reordered to show potential drop locations.

