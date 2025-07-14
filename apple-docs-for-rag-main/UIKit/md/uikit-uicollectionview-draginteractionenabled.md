

- UIKit
- UICollectionView
-  dragInteractionEnabled 

Instance Property

# dragInteractionEnabled

A Boolean value that indicates whether the collection view supports dragging content.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var dragInteractionEnabled: Bool { get set }
```

## Discussion

To support dragging content from the collection view to a view in your app or another app, set this property value to true. To disable this behavior, set the value to false. The default value is true.

In iOS 14 and earlier, the default value is true for iPad and false for iPhone. Setting the value to true on iPhone enables dragging within your app only. Dragging content to other apps isn’t possible on iPhone prior to iOS 15.

## See Also

### Managing drag interactions

var dragDelegate: (any UICollectionViewDragDelegate)?

The delegate object that manages the dragging of items from the collection view.

protocol UICollectionViewDragDelegate

The interface for initiating drags from a collection view.

var hasActiveDrag: Bool

A Boolean value that indicates whether items were lifted from the collection view and have not yet been dropped.

