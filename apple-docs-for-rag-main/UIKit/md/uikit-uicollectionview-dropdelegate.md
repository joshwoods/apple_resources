

- UIKit
- UICollectionView
-  dropDelegate 

Instance Property

# dropDelegate

The delegate object that manages the dropping of items into the collection view.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
weak var dropDelegate: (any UICollectionViewDropDelegate)? { get set }
```

## Mentioned in 

Supporting Drag and Drop in Collection Views

## See Also

### Managing drop interactions

protocol UICollectionViewDropDelegate

The interface for handling drops in a collection view.

var hasActiveDrop: Bool

A Boolean value that indicates whether the collection view is currently tracking a drop session.

var reorderingCadence: UICollectionView.ReorderingCadence

The speed at which items in the collection view are reordered to show potential drop locations.

enum ReorderingCadence

Constants indicating the speed at which collection view items are reorganized during a drop.

