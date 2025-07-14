

- Core Animation
- CADisplayLink
-  isPaused 

Instance Property

# isPaused

A Boolean value that indicates whether the system suspends the display link’s notifications to the target.

iOS 3.1+iPadOS 3.1+Mac Catalyst 13.1+macOS 14.0+tvOS 9.0+visionOS 1.0+

``` source
var isPaused: Bool { get set }
```

## Discussion

The default value is false. If true, the display link doesn’t send notifications to the target.

This property is thread safe, so you can set it from a thread separate to the one in which the display link runs.

## See Also

### Configuring a Display Link

var duration: CFTimeInterval

The time interval between screen refresh updates.

var preferredFrameRateRange: CAFrameRateRange

A range of frequencies your app allows for frame updates, affecting how often the system invokes your delegate’s callback.

var preferredFramesPerSecond: Int

A frequency your app prefers for frame updates, affecting how often the system invokes your delegate’s callback.

Deprecated

var timestamp: CFTimeInterval

The time interval that represents when the last frame displayed.

var targetTimestamp: CFTimeInterval

The time interval that represents when the next frame displays.

var frameInterval: Int

The number of frames that must pass before the display link notifies the target again.

Deprecated

