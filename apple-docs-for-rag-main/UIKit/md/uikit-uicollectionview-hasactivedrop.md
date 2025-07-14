

- UIKit
- UICollectionView
-  hasActiveDrop 

Instance Property

# hasActiveDrop

A Boolean value that indicates whether the collection view is currently tracking a drop session.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var hasActiveDrop: Bool { get }
```

## See Also

### Managing drop interactions

var dropDelegate: (any UICollectionViewDropDelegate)?

The delegate object that manages the dropping of items into the collection view.

protocol UICollectionViewDropDelegate

The interface for handling drops in a collection view.

var reorderingCadence: UICollectionView.ReorderingCadence

The speed at which items in the collection view are reordered to show potential drop locations.

enum ReorderingCadence

Constants indicating the speed at which collection view items are reorganized during a drop.

