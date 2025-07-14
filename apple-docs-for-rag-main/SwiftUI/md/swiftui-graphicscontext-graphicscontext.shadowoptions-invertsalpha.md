

- SwiftUI
- GraphicsContext
- GraphicsContext.ShadowOptions
-  invertsAlpha 

Type Property

# invertsAlpha

An option that causes the filter to invert the alpha of the shadow.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static var invertsAlpha: GraphicsContext.ShadowOptions { get }
```

## Discussion

You can create an “inner shadow” effect by combining this option with shadowAbove and using the sourceAtop blend mode.

## See Also

### Getting shadow options

static var disablesGroup: GraphicsContext.ShadowOptions

An option that causes the filter to composite the object and its shadow separately in the current layer.

static var shadowAbove: GraphicsContext.ShadowOptions

An option that causes the filter to draw the shadow above the object, rather than below it.

static var shadowOnly: GraphicsContext.ShadowOptions

An option that causes the filter to draw only the shadow, and omit the source object.

