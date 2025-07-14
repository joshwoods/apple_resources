

- Core Animation
- CADisplayLink
-  preferredFramesPerSecond Deprecated

Instance Property

# preferredFramesPerSecond

A frequency your app prefers for frame updates, affecting how often the system invokes your delegate’s callback.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0–2.4Deprecated

``` source
var preferredFramesPerSecond: Int { get set }
```

Deprecated

Use preferredFrameRateRange instead.

## Mentioned in 

Optimizing ProMotion refresh rates for iPhone 13 Pro and iPad Pro

## Discussion

The display link makes a best attempt to invoke your app’s callback at the frequency value you set to this property. However, the system also takes into account the device’s hardware capabilities and the other tasks your game or app is running.

Important

Choose a frame rate that your app can consistently maintain.

In iOS 15 and later, the system can change the available range of frame rates because it factors in system policies and a person’s preferences. For example, Low Power Mode, critical thermal state, and accessibility settings can affect the system’s frame rate.

The system typically provides a consistent frame rate by choosing one that’s a factor of the display’s maximum refresh rate. For example, a display link could invoke your callback 60 times per second for a display with a refresh rate of 60 hertz. However, the display link could invoke your callback less frequently, such as 30, 20, or 15 times per second, by setting a smaller value.

Note

The property defaults to `0`, which is equivalent to the display’s maximum refresh rate, such as a UIScreen instance’s maximumFramesPerSecond property.

See Optimizing ProMotion refresh rates for iPhone 13 Pro and iPad Pro for more information.

## See Also

### Configuring a Display Link

var duration: CFTimeInterval

The time interval between screen refresh updates.

var preferredFrameRateRange: CAFrameRateRange

A range of frequencies your app allows for frame updates, affecting how often the system invokes your delegate’s callback.

var isPaused: Bool

A Boolean value that indicates whether the system suspends the display link’s notifications to the target.

var timestamp: CFTimeInterval

The time interval that represents when the last frame displayed.

var targetTimestamp: CFTimeInterval

The time interval that represents when the next frame displays.

var frameInterval: Int

The number of frames that must pass before the display link notifies the target again.

Deprecated

