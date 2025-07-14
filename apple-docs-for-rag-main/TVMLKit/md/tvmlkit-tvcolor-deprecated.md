

- TVMLKit
-  TVColor Deprecated

Class

# TVColor

The color data used by styles.

tvOS 9.0–18.0Deprecated

``` source
class TVColor
```

Deprecated

Please use SwiftUI or UIKit

## Topics

### Getting Color Properties

var color: UIColor?

A UIColor object used to color an element.

var colorType: TVColorType

The color type for an element.

enum TVColorType

Designates how color for an element is to be displayed.

var gradientColors: [UIColor]?

An array of colors used to create a gradient for an element.

var gradientPoints: [NSNumber]?

An array of points used to determine gradient color changes.

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

## See Also

### Custom Styles

class TVViewElementStyle

A style applied to a view element.

Deprecated

class TVStyleFactory

An object used to register custom style properties.

Deprecated

