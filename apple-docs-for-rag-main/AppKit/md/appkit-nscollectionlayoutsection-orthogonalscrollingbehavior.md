

- AppKit
- NSCollectionLayoutSection
-  orthogonalScrollingBehavior 

Instance Property

# orthogonalScrollingBehavior

The section’s scrolling behavior in relation to the main layout axis.

macOS 10.15+

``` source
@MainActor
var orthogonalScrollingBehavior: NSCollectionLayoutSectionOrthogonalScrollingBehavior { get set }
```

## Discussion

The default value of this property is UICollectionLayoutSectionOrthogonalScrollingBehavior.none, which means the section lays out its content along the main axis of its layout, defined by the layout configuration’s scrollDirection property. Set a different value for this property to get the section to lay out its content orthogonally to the main layout axis.

