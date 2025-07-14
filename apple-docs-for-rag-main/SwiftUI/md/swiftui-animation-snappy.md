

- SwiftUI
- Animation
-  snappy 

Type Property

# snappy

A spring animation with a predefined duration and small amount of bounce that feels more snappy.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static var snappy: Animation { get }
```

## See Also

### Getting built-in spring animations

static var bouncy: Animation

A spring animation with a predefined duration and higher amount of bounce.

static func bouncy(duration: TimeInterval, extraBounce: Double) -> Animation

A spring animation with a predefined duration and higher amount of bounce that can be tuned.

static var smooth: Animation

A smooth spring animation with a predefined duration and no bounce.

static func smooth(duration: TimeInterval, extraBounce: Double) -> Animation

A smooth spring animation with a predefined duration and no bounce that can be tuned.

static func snappy(duration: TimeInterval, extraBounce: Double) -> Animation

A spring animation with a predefined duration and small amount of bounce that feels more snappy and can be tuned.

