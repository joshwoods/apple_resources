

- UIKit
- NSCollectionLayoutDimension
-  absolute(\_:) 

Type Method

# absolute(\_:)

Creates a dimension with an absolute point value.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
class func absolute(_ absoluteDimension: CGFloat) -> Self
```

## See Also

### Creating a dimension

class func estimated(CGFloat) -> Self

Creates a dimension with an estimated point value.

class func fractionalHeight(CGFloat) -> Self

Creates a dimension that is computed as a fraction of the height of the containing group.

class func fractionalWidth(CGFloat) -> Self

Creates a dimension that is computed as a fraction of the width of the containing group.

class func uniformAcrossSiblings(estimate: CGFloat) -> Self

Creates a dimension in which each item receives as much room as it requires and grows to match the dimension of its largest sibling.

