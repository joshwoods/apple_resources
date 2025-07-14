

- UIKit
-  UIDisplayGamut 

Enumeration

# UIDisplayGamut

Constants that indicate the gamut of the current display.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
enum UIDisplayGamut
```

## Topics

### Constants

case unspecified

An unspecified gamut value.

case SRGB

The sRGB display gamut.

case P3

The P3 display gamut.

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

### Retrieving display-related traits

var displayScale: CGFloat

The display scale of the trait collection.

var displayGamut: UIDisplayGamut

The gamut of the current display.

