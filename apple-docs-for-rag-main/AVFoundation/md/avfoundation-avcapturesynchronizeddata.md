

- AVFoundation
-  AVCaptureSynchronizedData 

Class

# AVCaptureSynchronizedData

The abstract superclass for media samples collected using synchronized capture.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
class AVCaptureSynchronizedData
```

## Topics

### Correlating Synchronized Data

var timestamp: CMTime

The time at which this synchronized data was captured.

## Relationships

### Inherits From

- NSObject

### Inherited By

- AVCaptureSynchronizedDepthData
- AVCaptureSynchronizedMetadataObjectData
- AVCaptureSynchronizedSampleBufferData

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

class AVCaptureSynchronizedDepthData

A container for scene depth information collected using synchronized capture.

