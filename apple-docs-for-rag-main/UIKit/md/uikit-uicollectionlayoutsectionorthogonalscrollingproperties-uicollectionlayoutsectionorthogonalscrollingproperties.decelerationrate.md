

- UIKit
- UICollectionLayoutSectionOrthogonalScrollingProperties
-  UICollectionLayoutSectionOrthogonalScrollingProperties.DecelerationRate 

Structure

# UICollectionLayoutSectionOrthogonalScrollingProperties.DecelerationRate

Constants that specify the rate of deceleration in the orthogonal scrolling section after the scrolling pan gesture ends.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
struct DecelerationRate
```

## Topics

### Selecting deceleration rates

static let automatic: UICollectionLayoutSectionOrthogonalScrollingProperties.DecelerationRate

A deceleration rate that matches the parent scroll view’s deceleration rate for the orthogonal scrolling section.

static let fast: UICollectionLayoutSectionOrthogonalScrollingProperties.DecelerationRate

A rapid deceleration rate for the orthogonal scrolling section.

static let normal: UICollectionLayoutSectionOrthogonalScrollingProperties.DecelerationRate

The default deceleration rate for the orthogonal scrolling section.

### Creating a deceleration rate

init(rawValue: CGFloat)

Creates a deceleration rate.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Specifying the rate of deceleration

var decelerationRate: UICollectionLayoutSectionOrthogonalScrollingProperties.DecelerationRate

A value that specifies the rate of deceleration in the orthogonal scrolling section after the scrolling pan gesture ends.

