

- Video Toolbox
- VTMotionBlurConfiguration
-  frameSupportedPixelFormats 

Instance Property

# frameSupportedPixelFormats

A list of source frame supported pixel formats for the current configuration.

macOS 15.4+

``` source
var frameSupportedPixelFormats: [NSNumber] { get }
```

## See Also

### Inspecting the configuration

var frameWidth: Int

The width of a source frame in pixels.

var frameHeight: Int

The height of a source frame in pixels.

var destinationPixelBufferAttributes: [String : any Sendable]

A dictionary of pixel buffer attributes describing the requirements for pixel buffers used as destination frames.

var sourcePixelBufferAttributes: [String : any Sendable]

A dictionary of pixel buffer attributes describing requirements for pixel buffers used as source frames and reference frames.

var qualityPrioritization: VTMotionBlurConfiguration.QualityPrioritization

A value that specifies whether to prioritize quality or performance.

enum QualityPrioritization

Values that specify whether to prioritize quality or performance.

var usePrecomputedFlow: Bool

A Boolean value to indicates whether the the optical flow will be provided by the user.

