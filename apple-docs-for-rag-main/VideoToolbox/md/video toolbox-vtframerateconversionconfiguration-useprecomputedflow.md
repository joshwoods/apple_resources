

- Video Toolbox
- VTFrameRateConversionConfiguration
-  usePrecomputedFlow 

Instance Property

# usePrecomputedFlow

A Boolean value to indicates whether the optical flow will be provided by the user.

macOS 15.4+

``` source
var usePrecomputedFlow: Bool { get }
```

## Discussion

If `false` this configuration computes the optical flow on the fly.

## See Also

### Inspecting the configuration

var frameWidth: Int

The width of a source frame in pixels.

var frameHeight: Int

The height of a source frame in pixels.

var sourcePixelBufferAttributes: [String : any Sendable]

A dictionary of pixel buffer attributes describing requirements for pixel buffers used as source frames and reference frames.

var destinationPixelBufferAttributes: [String : any Sendable]

A dictionary of pixel buffer attributes describing the requirements for pixel buffers used as destination frames.

var frameSupportedPixelFormats: [NSNumber]

A list of source frame supported pixel formats for the current configuration.

var qualityPrioritization: VTFrameRateConversionConfiguration.QualityPrioritization

A value that specifies whether to prioritize quality or performance.

enum QualityPrioritization

Values that specify whether to prioritize quality or performance.

