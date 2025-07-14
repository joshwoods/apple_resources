

- Vision
-  VisionError 

Enumeration

# VisionError

The errors that the framework produces.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
enum VisionError
```

## Topics

### Getting the error

case internalError(String)

An error that indicates the framework produces an internal error.

case ioError(String)

An error that indicates an I/O problem for an image, image sequence, or Core ML model.

case operationFailed(String)

An error that indicates the operation you request fails.

case outOfBoundsError(String)

An error that indicates an app attempts to access data that’s out-of-bounds.

case outOfMemory(String)

An error that indicates there’s not enough memory to perform the operation.

case pixelBufferCreationFailed(CVReturn)

An error that indicates a problem occurs when creating a pixel buffer.

case requestCancelled(String)

An error that indicates an app cancels the request.

case timeStampNotFound(String)

An error that indicates the system can’t find a timestamp.

case timeout(String)

An error that indicates an operation times out.

### Getting the invalid error

case invalidArgument(String)

An error that indicates a request has an invalid value.

case invalidFormat(String)

An error that indicates a request has data that’s formatted incorrectly.

case invalidImage(String)

An error that indicates the input image is invalid.

case invalidModel(String)

An error that indicates the Core ML model isn’t compatible with the request.

case invalidOperation(String)

An error that indicates an app requests an unsupported operation.

### Getting the data-unavailable error

case dataUnavailable(String)

An error that indicates the required data is missing.

### Getting the unsupported error

case unsupportedComputeDevice(String)

An error that indicates an app requests a compute device the framework doesn’t support.

case unsupportedComputeStage(String)

An error that indicates an app requests a compute stage the framework doesn’t support.

case unsupportedRequest(String)

An error that indicates an app attempts a request the framework doesn’t support.

case unsupportedRevision(String)

An error that indicates an app specifies a request revision the framework doesn’t support.

### Instance Properties

var description: String

## Relationships

### Conforms To

- Copyable
- Error
- LocalizedError
- Sendable

