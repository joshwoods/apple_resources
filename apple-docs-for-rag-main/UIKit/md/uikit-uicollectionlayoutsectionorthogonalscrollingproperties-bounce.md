

- UIKit
- UICollectionLayoutSectionOrthogonalScrollingProperties
-  bounce 

Instance Property

# bounce

A value that specifies whether the orthogonal scrolling section bounces past the edge of content and back again.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+tvOS 17.0+visionOS 1.0+

``` source
@MainActor
var bounce: UICollectionLayoutSectionOrthogonalScrollingProperties.Bounce { get set }
```

## Discussion

Set this value to specify whether the section stops scrolling immediately upon encountering the content boundary, or if it continues scrolling past the boundary and then bounces back.

## See Also

### Specifying the bounce behavior

enum Bounce

Constants that specify whether the orthogonal scrolling section bounces past the edge of content and back again.

