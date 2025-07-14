

- AppKit
- NSCollectionViewTransitionLayout
-  currentLayout 

Instance Property

# currentLayout

The collection view’s current layout object.

macOS 10.11+

``` source
@MainActor
var currentLayout: NSCollectionViewLayout { get }
```

## Discussion

Use this object to retrieve the initial layout attributes for elements of the collection view. If the transition is ultimately cancelled, the collection view animates its items back to the attributes provided by this object.

## See Also

### Accessing the Layout Objects

var nextLayout: NSCollectionViewLayout

The collection view’s new layout object.

