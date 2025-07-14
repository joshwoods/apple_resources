

- Core Animation
- CADisplayLink
-  duration 

Instance Property

# duration

The time interval between screen refresh updates.

iOS 3.1+iPadOS 3.1+Mac Catalyst 13.1+macOS 14.0+tvOS 9.0+visionOS 1.0+

``` source
var duration: CFTimeInterval { get }
```

## Discussion

This value is in an undefined state until the system calls the target’s selector at least once.

You calculate the expected amount of time your app has to render each frame by using targetTimestamp-timestamp. Use targetTimestamp-CACurrentMediaTime() to calculate the actual amount of time.

## See Also

### Configuring a Display Link

var preferredFrameRateRange: CAFrameRateRange

A range of frequencies your app allows for frame updates, affecting how often the system invokes your delegate’s callback.

var preferredFramesPerSecond: Int

A frequency your app prefers for frame updates, affecting how often the system invokes your delegate’s callback.

Deprecated

var isPaused: Bool

A Boolean value that indicates whether the system suspends the display link’s notifications to the target.

var timestamp: CFTimeInterval

The time interval that represents when the last frame displayed.

var targetTimestamp: CFTimeInterval

The time interval that represents when the next frame displays.

var frameInterval: Int

The number of frames that must pass before the display link notifies the target again.

Deprecated

