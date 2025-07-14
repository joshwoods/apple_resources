

- Video Toolbox
-  VTFrameRateConversionConfiguration 

Class

# VTFrameRateConversionConfiguration

An object that enables the frame rate conversion on a frame processing session.

macOS 15.4+

``` source
class VTFrameRateConversionConfiguration
```

## Topics

### Creating a frame rate conversion configuration

init?(frameWidth: Int, frameHeight: Int, usePrecomputedFlow: Bool, qualityPrioritization: VTFrameRateConversionConfiguration.QualityPrioritization, revision: VTFrameRateConversionConfiguration.Revision)

Creates a new frame rate conversion configuration with specified flow width and height.

### Determining processor availability

class var processorSupported: Bool

A Boolean value that indicates whether the processor supported on the current configuration.

### Inspecting the configuration

var frameWidth: Int

The width of a source frame in pixels.

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

### Inspecting revision information

var revision: VTFrameRateConversionConfiguration.Revision

The specific algorithm or configuration revision to use to perform the request.

class var defaultRevision: VTFrameRateConversionConfiguration.Revision

The default revision of a particular algorithm or configuration.

class var supportedRevisions: IndexSet

The collection of currently-supported algorithms or configuration revisions for the class of configurations.

enum Revision

The specific algorithm or configuration revision that is to be used to perform the request.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable
- VTFrameProcessorConfiguration

## See Also

### Frame rate conversion

class VTFrameRateConversionParameters

An object that contains the required input and output parameters to run a frame rate conversion processor on a frame.

