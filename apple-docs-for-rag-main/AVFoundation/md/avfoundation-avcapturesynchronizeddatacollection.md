

- AVFoundation
-  AVCaptureSynchronizedDataCollection 

Class

# AVCaptureSynchronizedDataCollection

A set of data samples collected simultaneously from multiple capture outputs.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
class AVCaptureSynchronizedDataCollection
```

## Topics

### Accessing Synchronized Data

var count: Int

The number of synchronized data objects in the collection.

func synchronizedData(for: AVCaptureOutput) -> AVCaptureSynchronizedData?

Returns synchronized data captured by the specified capture output.

subscript(AVCaptureOutput) -> AVCaptureSynchronizedData?

Returns data captured by the specified capture output, using subscript syntax.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSFastEnumeration
- NSObjectProtocol
- Sequence

## See Also

### Synchronized capture

class AVCaptureDataOutputSynchronizer

An object that coordinates time-matched delivery of data from multiple capture outputs.

class AVCaptureSynchronizedSampleBufferData

A container for video or audio samples collected using synchronized capture.

class AVCaptureSynchronizedMetadataObjectData

A container for metadata objects collected using synchronized capture.

class AVCaptureSynchronizedDepthData

A container for scene depth information collected using synchronized capture.

class AVCaptureSynchronizedData

The abstract superclass for media samples collected using synchronized capture.

