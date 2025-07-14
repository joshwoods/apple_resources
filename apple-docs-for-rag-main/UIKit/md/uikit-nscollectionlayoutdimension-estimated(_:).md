

- UIKit
- NSCollectionLayoutDimension
-  estimated(\_:) 

Type Method

# estimated(\_:)

Creates a dimension with an estimated point value.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

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

class func uniformAcrossSiblings(estimate: CGFloat) -> Self

Creates a dimension in which each item receives as much room as it requires and grows to match the dimension of its largest sibling.

