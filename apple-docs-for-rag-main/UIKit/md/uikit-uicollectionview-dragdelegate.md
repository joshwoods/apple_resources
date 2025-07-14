

- UIKit
- UICollectionView
-  dragDelegate 

Instance Property

# dragDelegate

The delegate object that manages the dragging of items from the collection view.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
weak var dragDelegate: (any UICollectionViewDragDelegate)? { get set }
```

## Mentioned in 

Supporting Drag and Drop in Collection Views

## See Also

### Managing drag interactions

protocol UICollectionViewDragDelegate

The interface for initiating drags from a collection view.

var hasActiveDrag: Bool

A Boolean value that indicates whether items were lifted from the collection view and have not yet been dropped.

var dragInteractionEnabled: Bool

A Boolean value that indicates whether the collection view supports dragging content.

