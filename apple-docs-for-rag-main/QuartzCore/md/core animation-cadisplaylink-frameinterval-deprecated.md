

- Core Animation
- CADisplayLink
-  frameInterval Deprecated

Instance Property

# frameInterval

The number of frames that must pass before the display link notifies the target again.

iOS 3.1–10.0DeprecatediPadOS 3.1–10.0DeprecatedMac Catalyst 13.1–13.1DeprecatedtvOS 9.0–10.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
var frameInterval: Int { get set }
```

Deprecated

Use preferredFramesPerSecond instead.

## Discussion

The default value is `1`, which results in the system notifying your app at the refresh rate of the display. If you set the value to a value greater than `1`, the display link notifies your app at a fraction of the native refresh rate. For example, setting the interval to `2` causes the display link to fire every other frame, providing half the frame rate.

Setting this value to less than `1` results in undefined behavior and is a programmer error.

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

var timestamp: CFTimeInterval

The time interval that represents when the last frame displayed.

var targetTimestamp: CFTimeInterval

The time interval that represents when the next frame displays.

