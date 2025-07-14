

- UIKit
- UICollectionLayoutSectionOrthogonalScrollingProperties
-  UICollectionLayoutSectionOrthogonalScrollingProperties.Bounce 

Enumeration

# UICollectionLayoutSectionOrthogonalScrollingProperties.Bounce

Constants that specify whether the orthogonal scrolling section bounces past the edge of content and back again.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+tvOS 17.0+visionOS 1.0+

``` source
enum Bounce
```

## Topics

### Selecting bounce options

case always

The orthogonal scroll view bounces even if the content is smaller than its bounds.

case automatic

The orthogonal scroll view bounces when it encounters a content boundary.

case never

The orthogonal scroll view stops scrolling immediately when it encounters a content boundary without bouncing.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Specifying the bounce behavior

var bounce: UICollectionLayoutSectionOrthogonalScrollingProperties.Bounce

A value that specifies whether the orthogonal scrolling section bounces past the edge of content and back again.

