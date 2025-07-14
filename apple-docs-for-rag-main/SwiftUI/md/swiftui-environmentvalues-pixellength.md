

- SwiftUI
- EnvironmentValues
-  pixelLength 

Instance Property

# pixelLength

The size of a pixel on the screen.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var pixelLength: CGFloat { get }
```

## Discussion

This value is usually equal to `1` divided by displayScale.

## See Also

### Reacting to interface characteristics

var isLuminanceReduced: Bool

A Boolean value that indicates whether the display or environment currently requires reduced luminance.

var displayScale: CGFloat

The display scale of this environment.

var horizontalSizeClass: UserInterfaceSizeClass?

The horizontal size class of this environment.

var verticalSizeClass: UserInterfaceSizeClass?

The vertical size class of this environment.

enum UserInterfaceSizeClass

A set of values that indicate the visual size available to the view.

