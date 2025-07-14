

- Video Toolbox
- VTFrameRateConversionConfiguration
-  frameWidth 

Instance Property

# frameWidth

The width of a source frame in pixels.

macOS 15.4+

``` source
var frameWidth: Int { get }
```

## Discussion

The maximum value is 8192 pixels for macOS, and 4096 pixels for iOS.

## See Also

### Inspecting the configuration

var frameHeight: Int

The height of a source frame in pixels.

var usePrecomputedFlow: Bool

A Boolean value to indicates whether the optical flow will be provided by the user.

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

