

- UIKit
-  UICollectionLayoutSectionOrthogonalScrollingProperties 

Class

# UICollectionLayoutSectionOrthogonalScrollingProperties

An object that specifies properties for a layout section that scrolls orthogonally in relation to the main layout axis.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+tvOS 17.0+visionOS 1.0+

``` source
@MainActor
class UICollectionLayoutSectionOrthogonalScrollingProperties
```

## Topics

### Specifying the bounce behavior

var bounce: UICollectionLayoutSectionOrthogonalScrollingProperties.Bounce

A value that specifies whether the orthogonal scrolling section bounces past the edge of content and back again.

enum Bounce

Constants that specify whether the orthogonal scrolling section bounces past the edge of content and back again.

### Specifying the rate of deceleration

var decelerationRate: UICollectionLayoutSectionOrthogonalScrollingProperties.DecelerationRate

A value that specifies the rate of deceleration in the orthogonal scrolling section after the scrolling pan gesture ends.

struct DecelerationRate

Constants that specify the rate of deceleration in the orthogonal scrolling section after the scrolling pan gesture ends.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol
- Sendable

## See Also

### Specifying scrolling behavior

var orthogonalScrollingBehavior: UICollectionLayoutSectionOrthogonalScrollingBehavior

The section’s scrolling behavior in relation to the main layout axis.

var orthogonalScrollingProperties: UICollectionLayoutSectionOrthogonalScrollingProperties

The section’s orthogonal scrolling properties.

