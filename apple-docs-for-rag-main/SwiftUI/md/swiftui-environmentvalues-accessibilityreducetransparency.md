

- SwiftUI
- EnvironmentValues
-  accessibilityReduceTransparency 

Instance Property

# accessibilityReduceTransparency

Whether the system preference for Reduce Transparency is enabled.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var accessibilityReduceTransparency: Bool { get }
```

## Discussion

If this property’s value is true, UI (mainly window) backgrounds should not be semi-transparent; they should be opaque.

## See Also

### Improving legibility

var accessibilityShowButtonShapes: Bool

Whether the system preference for Show Button Shapes is enabled.

var legibilityWeight: LegibilityWeight?

The font weight to apply to text.

enum LegibilityWeight

The Accessibility Bold Text user setting options.

