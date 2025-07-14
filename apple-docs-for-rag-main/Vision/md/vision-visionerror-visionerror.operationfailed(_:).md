

- Vision
- VisionError
-  VisionError.operationFailed(\_:) 

Case

# VisionError.operationFailed(\_:)

An error that indicates the operation you request fails.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
case operationFailed(String)
```

## See Also

### Getting the error

case internalError(String)

An error that indicates the framework produces an internal error.

case ioError(String)

An error that indicates an I/O problem for an image, image sequence, or Core ML model.

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

