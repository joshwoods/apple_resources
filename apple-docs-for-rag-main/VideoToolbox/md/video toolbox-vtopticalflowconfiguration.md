

- Video Toolbox
-  VTOpticalFlowConfiguration 

Class

# VTOpticalFlowConfiguration

A configuration object that enables optical flow on a frame processing session.

macOS 15.4+

``` source
class VTOpticalFlowConfiguration
```

## Topics

### Creating an optical flow configuration

init?(frameWidth: Int, frameHeight: Int, qualityPrioritization: VTOpticalFlowConfiguration.QualityPrioritization, revision: VTOpticalFlowConfiguration.Revision)

### Determining processor availability

class var processorSupported: Bool

A boolean value that indicates whether the processor supported on the current configuration.

### Inspecting the configuration

var frameWidth: Int

The width of a source frame in pixels.

var frameHeight: Int

The height of source frame in pixels.

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

### Inspecting revision information

var revision: VTOpticalFlowConfiguration.Revision

The specific algorithm or configuration revision that is to be used to perform the request.

class var defaultRevision: VTOpticalFlowConfiguration.Revision

The default revision of a particular algorithm or configuration.

class var supportedRevisions: IndexSet

A boolean value that indicates whether the processor supported on the current configuration.

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

### Optical flow

class VTFrameProcessorOpticalFlow

A class to wrap bidirectional optical flow to send to the processor.

class VTOpticalFlowParameters

An object that describes frame-level optical flow parameters.

