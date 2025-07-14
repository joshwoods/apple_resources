

- AVFoundation
-  AVCaptureSynchronizedSampleBufferData 

Class

# AVCaptureSynchronizedSampleBufferData

A container for video or audio samples collected using synchronized capture.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
class AVCaptureSynchronizedSampleBufferData
```

## Topics

### Accessing Synchronized Data

var sampleBuffer: CMSampleBuffer

The depth data captured at this synchronization point.

### Handling Dropped Data

var sampleBufferWasDropped: Bool

A Boolean value indicating whether sample buffers were discarded between capture and processing.

var droppedReason: AVCaptureOutput.DataDroppedReason

A value indicating why the capture output failed to deliver sample buffers, if applicable.

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

class AVCaptureSynchronizedMetadataObjectData

A container for metadata objects collected using synchronized capture.

class AVCaptureSynchronizedDepthData

A container for scene depth information collected using synchronized capture.

class AVCaptureSynchronizedData

The abstract superclass for media samples collected using synchronized capture.

