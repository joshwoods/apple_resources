

- SwiftUI
- GraphicsContext
- GraphicsContext.GradientOptions
-  mirror 

Type Property

# mirror

An option that repeats the gradient outside its nominal range, reflecting every other instance.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static var mirror: GraphicsContext.GradientOptions { get }
```

## Discussion

Use this option to cause the gradient to repeat its pattern in areas that exceed the bounds of its start and end points. The repetitions alternately reverse the start and end points, producing a pattern like `0 -> 1`, `1 -> 0`, `0 -> 1`, and so on.

Without either this option or repeat, the gradient stops at the end of its range. This option takes precendence if you set both this one and repeat.

## See Also

### Getting gradient options

static var linearColor: GraphicsContext.GradientOptions

An option that interpolates between colors in a linear color space.

static var `repeat`: GraphicsContext.GradientOptions

An option that repeats the gradient outside its nominal range.

