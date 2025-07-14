

- AppKit
- NSCollectionLayoutDimension
-  estimated(\_:) 

Type Method

# estimated(\_:)

Creates a dimension with an estimated point value.

macOS 10.15+

``` source
@MainActor
class func estimated(_ estimatedDimension: CGFloat) -> Self
```

## Discussion

The final size of the dimension is determined when the content is rendered.

## See Also

### Creating a dimension

class func absolute(CGFloat) -> Self

Creates a dimension with an absolute point value.

class func fractionalHeight(CGFloat) -> Self

Creates a dimension that is computed as a fraction of the height of the containing group.

class func fractionalWidth(CGFloat) -> Self

Creates a dimension that is computed as a fraction of the width of the containing group.

