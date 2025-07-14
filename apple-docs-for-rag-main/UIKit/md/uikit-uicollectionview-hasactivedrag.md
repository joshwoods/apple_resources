

- UIKit
- UICollectionView
-  hasActiveDrag 

Instance Property

# hasActiveDrag

A Boolean value that indicates whether items were lifted from the collection view and have not yet been dropped.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var hasActiveDrag: Bool { get }
```

## See Also

### Managing drag interactions

var dragDelegate: (any UICollectionViewDragDelegate)?

The delegate object that manages the dragging of items from the collection view.

protocol UICollectionViewDragDelegate

The interface for initiating drags from a collection view.

var dragInteractionEnabled: Bool

A Boolean value that indicates whether the collection view supports dragging content.

