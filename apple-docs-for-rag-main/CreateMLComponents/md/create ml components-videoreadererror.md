

- Create ML Components
-  VideoReaderError 

Enumeration

# VideoReaderError

Video loader errors.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
enum VideoReaderError
```

## Topics

### Analyzing the error

case cameraAuthorizationDenied

An error that indicates that the camera authorization status is denied. The user has explicitly denied permission for media capture.

case cameraAuthorizationRestricted

An error that indicates that the camera authorization status is restricted. The user is not allowed to access media capture devices.

case frameRateNotSupported(Double)

An error that indicates that the frame rate is not supported by the input camera.

case missingVideoTrack(URL)

An error that indicates that the VideoReader cannot find a video track.

case sourceCameraNotAvailable

An error that indicates that no cameras are available.

var errorDescription: String?

A localized message describing what error occurred.

### Operators

static func == (VideoReaderError, VideoReaderError) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case captureSessionStopped

An error that indicates that the capture session stopped.

### Default Implementations

CustomDebugStringConvertible Implementations

Equatable Implementations

Error Implementations

LocalizedError Implementations

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- Equatable
- Error
- LocalizedError
- Sendable

## See Also

### Errors

enum AudioPreprocessingError

Audio preprocessing errors.

enum AudioReaderError

Audio reader errors.

enum CompatibilityError

A compatibility error.

enum ConcatenationError

Errors thrown when concatenating numeric values.

enum DatasetError

Dataset processing errors.

enum EstimatorEncodingError

An estimator encoding error.

enum ModelCompatibilityError

Errors related to CoreML model compatibility.

enum ModelUpdateError

An updatable model error.

enum OptimizationError

An optimization error.

enum PipelineDataError

Errors related to pipeline data affinity problems.

enum SerializationError

A serialization error.

enum TabularPipelineDataError

Errors related to tabular pipeline data affinity problems.

