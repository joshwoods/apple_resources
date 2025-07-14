

- TVMLKit
-  TVColorType Deprecated

Enumeration

# TVColorType

Designates how color for an element is to be displayed.

tvOS 9.0–18.0Deprecated

``` source
enum TVColorType
```

Deprecated

Please use SwiftUI or UIKit

## Topics

### Constants

case none

Indicates that there is no color associated with an element.

case plain

Indicates that a single color is to be used with an element.

case linearGradientTopToBottom

Indicates that a color gradient goes from the top to the bottom of an element.

case linearGradientLeftToRight

Indicates that a color gradient goes from the left to the right of an element.

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

### Getting Color Properties

var color: UIColor?

A UIColor object used to color an element.

Deprecated

var colorType: TVColorType

The color type for an element.

Deprecated

var gradientColors: [UIColor]?

An array of colors used to create a gradient for an element.

Deprecated

var gradientPoints: [NSNumber]?

An array of points used to determine gradient color changes.

Deprecated

