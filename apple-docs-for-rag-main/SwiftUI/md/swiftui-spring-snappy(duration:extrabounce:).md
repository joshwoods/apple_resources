

- SwiftUI
- Spring
-  snappy(duration:extraBounce:) 

Type Method

# snappy(duration:extraBounce:)

A spring with a predefined duration and small amount of bounce that feels more snappy and can be tuned.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
static func snappy(
    duration: TimeInterval = 0.5,
    extraBounce: Double = 0.0
) -> Spring
```

## Parameters 

`duration`  

The perceptual duration, which defines the pace of the spring. This is approximately equal to the settling duration, but for very bouncy springs, will be the duration of the period of oscillation for the spring.

`extraBounce`  

How much additional bounciness should be added to the base bounce of 0.15.

## See Also

### Getting built-in springs

static var bouncy: Spring

A spring with a predefined duration and higher amount of bounce.

static func bouncy(duration: TimeInterval, extraBounce: Double) -> Spring

A spring with a predefined duration and higher amount of bounce that can be tuned.

static var smooth: Spring

A smooth spring with a predefined duration and no bounce.

static func smooth(duration: TimeInterval, extraBounce: Double) -> Spring

A smooth spring with a predefined duration and no bounce that can be tuned.

static var snappy: Spring

A spring with a predefined duration and small amount of bounce that feels more snappy.

