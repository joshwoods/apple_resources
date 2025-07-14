

- Core Animation
- CAMetalDisplayLink
-  preferredFrameLatency 

Instance Property

# preferredFrameLatency

The amount of time, in frames, your app requests to render a frame.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
var preferredFrameLatency: Float { get set }
```

## Discussion

The final latency may be bigger if the system needs more time, such as for windowed modes on macOS.

Important

The only acceptable values are `1.0` and `2.0`.

## See Also

### Configuring a Display Link

var preferredFrameRateRange: CAFrameRateRange

A range of frequencies your app allows for frame updates, affecting how often the system invokes your delegate’s callback.

var delegate: (any CAMetalDisplayLinkDelegate)?

An instance of a type your app implements that responds to the system’s callbacks.

