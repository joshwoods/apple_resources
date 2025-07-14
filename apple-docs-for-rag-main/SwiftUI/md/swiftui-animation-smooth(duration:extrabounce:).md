

- SwiftUI
- Animation
-  smooth(duration:extraBounce:) 

Type Method

# smooth(duration:extraBounce:)

A smooth spring animation with a predefined duration and no bounce that can be tuned.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static func smooth(
    duration: TimeInterval = 0.5,
    extraBounce: Double = 0.0
) -> Animation
```

## Parameters 

`duration`  

The perceptual duration, which defines the pace of the spring. This is approximately equal to the settling duration, but for very bouncy springs, will be the duration of the period of oscillation for the spring.

`extraBounce`  

How much additional bounce should be added to the base bounce of 0.

## See Also

### Getting built-in spring animations

static var bouncy: Animation

A spring animation with a predefined duration and higher amount of bounce.

static func bouncy(duration: TimeInterval, extraBounce: Double) -> Animation

A spring animation with a predefined duration and higher amount of bounce that can be tuned.

static var smooth: Animation

A smooth spring animation with a predefined duration and no bounce.

static var snappy: Animation

A spring animation with a predefined duration and small amount of bounce that feels more snappy.

static func snappy(duration: TimeInterval, extraBounce: Double) -> Animation

A spring animation with a predefined duration and small amount of bounce that feels more snappy and can be tuned.

