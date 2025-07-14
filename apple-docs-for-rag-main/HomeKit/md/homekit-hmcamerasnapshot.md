

- HomeKit
-  HMCameraSnapshot 

Class

# HMCameraSnapshot

An object that represents a snapshot taken from a camera.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
class HMCameraSnapshot
```

## Topics

### Accessing snapshot properties

var captureDate: Date

Date and time at which the snapshot was requested.

### Initializers

init()Deprecated

## Relationships

### Inherits From

- HMCameraSource

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Taking snapshots

func takeSnapshot()

Takes an image snapshot.

var mostRecentSnapshot: HMCameraSnapshot?

The camera’s most recent snapshot.

