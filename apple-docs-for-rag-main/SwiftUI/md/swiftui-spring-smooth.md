

- SwiftUI
- Spring
-  smooth 

Type Property

# smooth

A smooth spring with a predefined duration and no bounce.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
static var smooth: Spring { get }
```

## See Also

### Getting built-in springs

static var bouncy: Spring

A spring with a predefined duration and higher amount of bounce.

static func bouncy(duration: TimeInterval, extraBounce: Double) -> Spring

A spring with a predefined duration and higher amount of bounce that can be tuned.

static func smooth(duration: TimeInterval, extraBounce: Double) -> Spring

A smooth spring with a predefined duration and no bounce that can be tuned.

static var snappy: Spring

A spring with a predefined duration and small amount of bounce that feels more snappy.

static func snappy(duration: TimeInterval, extraBounce: Double) -> Spring

A spring with a predefined duration and small amount of bounce that feels more snappy and can be tuned.

