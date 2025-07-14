

- SwiftUI
- GraphicsContext
- GraphicsContext.GradientOptions
-  repeat 

Type Property

# repeat

An option that repeats the gradient outside its nominal range.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static var `repeat`: GraphicsContext.GradientOptions { get }
```

## Discussion

Use this option to cause the gradient to repeat its pattern in areas that exceed the bounds of its start and end points. The repetitions use the same start and end value for each repetition.

Without this option or mirror, the gradient stops at the end of its range. The mirror option takes precendence if you set both this one and that one.

## See Also

### Getting gradient options

static var linearColor: GraphicsContext.GradientOptions

An option that interpolates between colors in a linear color space.

static var mirror: GraphicsContext.GradientOptions

An option that repeats the gradient outside its nominal range, reflecting every other instance.

