

- Video Toolbox
- VTOpticalFlowConfiguration
-  frameHeight 

Instance Property

# frameHeight

The height of source frame in pixels.

macOS 15.4+

``` source
var frameHeight: Int { get }
```

## Discussion

The maximum value is 8192 pixels for macOS, and 4096 pixels for iOS.

## See Also

### Inspecting the configuration

var frameWidth: Int

The width of a source frame in pixels.

var sourcePixelBufferAttributes: [String : any Sendable]

A dictionary of pixel buffer attributes describing requirements for pixel buffers used as source frames and reference frames.

var destinationPixelBufferAttributes: [String : any Sendable]

A dictionary of pixel buffer attributes describing the requirements for pixel buffers used as destination frames.

var frameSupportedPixelFormats: [NSNumber]

A list of source frame supported pixel formats for the current configuration.

var qualityPrioritization: VTOpticalFlowConfiguration.QualityPrioritization

A value that specifies whether to prioritize quality or performance.

enum QualityPrioritization

Values that specify whether to prioritize quality or performance.

