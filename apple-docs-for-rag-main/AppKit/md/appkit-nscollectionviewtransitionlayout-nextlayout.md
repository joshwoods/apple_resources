

- AppKit
- NSCollectionViewTransitionLayout
-  nextLayout 

Instance Property

# nextLayout

The collection view’s new layout object.

macOS 10.11+

``` source
@MainActor
var nextLayout: NSCollectionViewLayout { get }
```

## Discussion

Use this object to retrieve the final layout attributes for elements of the collection view. If the transition completes as expected, the collection view animates its items to the attributes provided by this object.

## See Also

### Accessing the Layout Objects

var currentLayout: NSCollectionViewLayout

The collection view’s current layout object.

