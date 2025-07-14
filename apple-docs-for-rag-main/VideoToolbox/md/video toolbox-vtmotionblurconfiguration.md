

- Video Toolbox
-  VTMotionBlurConfiguration 

Class

# VTMotionBlurConfiguration

A configuration object to enable motion blur on a frame processing session.

macOS 15.4+

``` source
class VTMotionBlurConfiguration
```

## Topics

### Creating a motion blur configuration

init?(frameWidth: Int, frameHeight: Int, usePrecomputedFlow: Bool, qualityPrioritization: VTMotionBlurConfiguration.QualityPrioritization, revision: VTMotionBlurConfiguration.Revision)

Creates a new motion blur configuration with specified flow width and height.

### Determining processor availability

class var processorSupported: Bool

A Boolean value that indicates whether the processor is supported.

### Inspecting the configuration

var frameWidth: Int

The width of a source frame in pixels.

var frameHeight: Int

The height of a source frame in pixels.

var frameSupportedPixelFormats: [NSNumber]

A list of source frame supported pixel formats for the current configuration.

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

### Inspecting revision information

var revision: VTMotionBlurConfiguration.Revision

The specific algorithm or configuration revision that is to be used to perform the request.

class var defaultRevision: VTMotionBlurConfiguration.Revision

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

### Motion blur

class VTMotionBlurParameters

This object contains both input and output parameters necessary to run the motion blur processor on a frame.

