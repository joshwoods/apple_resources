

- Core Animation
- CADisplayLink
-  timestamp 

Instance Property

# timestamp

The time interval that represents when the last frame displayed.

iOS 3.1+iPadOS 3.1+Mac Catalyst 13.1+macOS 14.0+tvOS 9.0+visionOS 1.0+

``` source
var timestamp: CFTimeInterval { get }
```

## Mentioned in 

Optimizing ProMotion refresh rates for iPhone 13 Pro and iPad Pro

## Discussion

If you need to calculate what to display next, use targetTimestamp instead.

## See Also

### Configuring a Display Link

var duration: CFTimeInterval

The time interval between screen refresh updates.

var preferredFrameRateRange: CAFrameRateRange

A range of frequencies your app allows for frame updates, affecting how often the system invokes your delegate’s callback.

var preferredFramesPerSecond: Int

A frequency your app prefers for frame updates, affecting how often the system invokes your delegate’s callback.

Deprecated

var isPaused: Bool

A Boolean value that indicates whether the system suspends the display link’s notifications to the target.

var targetTimestamp: CFTimeInterval

The time interval that represents when the next frame displays.

var frameInterval: Int

The number of frames that must pass before the display link notifies the target again.

Deprecated

