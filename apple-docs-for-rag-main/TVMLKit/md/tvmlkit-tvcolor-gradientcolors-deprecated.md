

- TVMLKit
- TVColor
-  gradientColors Deprecated

Instance Property

# gradientColors

An array of colors used to create a gradient for an element.

tvOS 9.0–18.0Deprecated

``` source
var gradientColors: [UIColor]? { get }
```

Deprecated

Please use SwiftUI or UIKit

## Discussion

This property is only available when colorType is set to TVColorType.linearGradientTopToBottom or TVColorType.linearGradientLeftToRight.

## See Also

### Getting Color Properties

var color: UIColor?

A UIColor object used to color an element.

Deprecated

var colorType: TVColorType

The color type for an element.

Deprecated

enum TVColorType

Designates how color for an element is to be displayed.

Deprecated

var gradientPoints: [NSNumber]?

An array of points used to determine gradient color changes.

Deprecated

