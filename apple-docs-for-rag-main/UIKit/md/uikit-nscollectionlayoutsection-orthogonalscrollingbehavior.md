

- UIKit
- NSCollectionLayoutSection
-  orthogonalScrollingBehavior 

Instance Property

# orthogonalScrollingBehavior

The section’s scrolling behavior in relation to the main layout axis.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
var orthogonalScrollingBehavior: UICollectionLayoutSectionOrthogonalScrollingBehavior { get set }
```

## Discussion

The default value of this property is UICollectionLayoutSectionOrthogonalScrollingBehavior.none, which means the section lays out its content along the main axis of its layout, defined by the layout configuration’s scrollDirection property. Set a different value for this property to get the section to lay out its content orthogonally to the main layout axis.

## See Also

### Specifying scrolling behavior

var orthogonalScrollingProperties: UICollectionLayoutSectionOrthogonalScrollingProperties

The section’s orthogonal scrolling properties.

class UICollectionLayoutSectionOrthogonalScrollingProperties

An object that specifies properties for a layout section that scrolls orthogonally in relation to the main layout axis.

