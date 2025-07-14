

- AVFoundation
-  AVCaptureSynchronizedDepthData 

Class

# AVCaptureSynchronizedDepthData

A container for scene depth information collected using synchronized capture.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
class AVCaptureSynchronizedDepthData
```

## Topics

### Accessing Synchronized Data

var depthData: AVDepthData

The depth data captured at this synchronization point.

### Handling Dropped Data

var depthDataWasDropped: Bool

A Boolean value indicating whether depth data was discarded between capture and processing.

var droppedReason: AVCaptureOutput.DataDroppedReason

A value indicating why the capture output failed to deliver depth data, if applicable.

## Relationships

### Inherits From

- AVCaptureSynchronizedData

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Synchronized capture

class AVCaptureDataOutputSynchronizer

An object that coordinates time-matched delivery of data from multiple capture outputs.

class AVCaptureSynchronizedDataCollection

A set of data samples collected simultaneously from multiple capture outputs.

class AVCaptureSynchronizedSampleBufferData

A container for video or audio samples collected using synchronized capture.

class AVCaptureSynchronizedMetadataObjectData

A container for metadata objects collected using synchronized capture.

class AVCaptureSynchronizedData

The abstract superclass for media samples collected using synchronized capture.

