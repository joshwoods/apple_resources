

- Core Animation
- CAMetalDisplayLink
-  delegate 

Instance Property

# delegate

An instance of a type your app implements that responds to the system’s callbacks.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
weak var delegate: (any CAMetalDisplayLinkDelegate)? { get set }
```

## See Also

### Configuring a Display Link

var preferredFrameRateRange: CAFrameRateRange

A range of frequencies your app allows for frame updates, affecting how often the system invokes your delegate’s callback.

var preferredFrameLatency: Float

The amount of time, in frames, your app requests to render a frame.

