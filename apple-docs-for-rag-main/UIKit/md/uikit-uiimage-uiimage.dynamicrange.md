

- UIKit
- UIImage
-  UIImage.DynamicRange 

Enumeration

# UIImage.DynamicRange

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+tvOS 17.0+visionOS 1.0+

``` source
enum DynamicRange
```

## Topics

### Enumeration Cases

case constrainedHigh

case high

case standard

case unspecified

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

### Specifying the dynamic range

var isHighDynamicRange: Bool

func imageRestrictedToStandardDynamicRange() -> UIImage

func heicData() -> Data?

