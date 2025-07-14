

- Vision
-  VNErrorCode 

Enumeration

# VNErrorCode

Constants that identify errors from the framework.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.0+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
enum VNErrorCode
```

## Topics

### Error Codes

case turiCoreErrorCode

An error occurred during Create ML training due to an invalid transformation or image.

case OK

The operation finished without error.

case dataUnavailable

The data isn’t available.

case internalError

An internal error occurred within the framework.

case invalidArgument

An app passed an invalid parameter to a request.

case invalidFormat

The format of the image is invalid.

case invalidImage

The image is invalid.

case invalidModel

The Core ML model is incompatible with the request.

case invalidOperation

An app requested an unsupported operation.

case invalidOption

An app specified an invalid option on a request.

case ioError

An I/O error for an image, image sequence, or Core ML model.

case missingOption

A request is missing a required option.

case notImplemented

The method isn’t implemented in the underlying model.

case operationFailed

The requested operation failed.

case outOfBoundsError

An app attempted to access data that’s out-of-bounds.

case outOfMemory

The system doesn’t have enough memory to complete the request.

case requestCancelled

An app canceled the request.

case timeStampNotFound

The system can’t find a timestamp.

case unknownError

An unidentified error occurred.

case unsupportedRevision

An app specified an unsupported request revision.

case unsupportedRequest

An app attempted an unsupported request.

case unsupportedComputeDevice

An app requested an unsupported compute device.

case unsupportedComputeStage

An app requested an unsupported compute stage.

case timeout

The requested operation timed out.

### Creating an Error Code

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Errors

let VNErrorDomain: String

The domain of errors that the framework generates.

