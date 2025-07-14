

- Core Animation
- CAMetalDisplayLink
-  preferredFrameRateRange 

Instance Property

# preferredFrameRateRange

A range of frequencies your app allows for frame updates, affecting how often the system invokes your delegate’s callback.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
var preferredFrameRateRange: CAFrameRateRange { get set }
```

## Discussion

The display link makes a best attempt to invoke your app’s callback within the frequency range you set to this property. However, the system also takes into account the device’s hardware capabilities and the other tasks your game or app is running.

Important

Choose a frame rate range that your app can consistently maintain.

The system can change the available range of frame rates because it factors in system policies and a person’s preferences. For example, Low Power Mode, critical thermal state, and accessibility settings can affect the system’s frame rate.

The system typically provides a consistent frame rate by choosing one that’s a factor of the display’s maximum refresh rate. For example, a display link could invoke your callback 60 times per second for a display with a refresh rate of 60 hertz. However, the display link could invoke your callback less frequently, such as 30, 20, or 15 hertz, by setting a range with smaller values.

Note

By default, this property’s values are equal to default, which is equivalent to the display’s maximum refresh rate, such as a UIScreen instance’s maximumFramesPerSecond property.

See Optimizing ProMotion refresh rates for iPhone 13 Pro and iPad Pro for more information.

## See Also

### Configuring a Display Link

var preferredFrameLatency: Float

The amount of time, in frames, your app requests to render a frame.

var delegate: (any CAMetalDisplayLinkDelegate)?

An instance of a type your app implements that responds to the system’s callbacks.

