

- UIKit
- UICollectionViewTransitionLayout
-  nextLayout 

Instance Property

# nextLayout

The collection view’s new layout object.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var nextLayout: UICollectionViewLayout { get }
```

## Discussion

This object provides the layout attributes representing the new position of items in the collection view. If the transition completes as expected, the collection view animates its items to the positions provided by this object.

## See Also

### Accessing the layout objects

var currentLayout: UICollectionViewLayout

The collection view’s current layout object.

