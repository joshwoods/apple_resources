

- HomeKit
-  HMCameraSource 

Class

# HMCameraSource

An abstract class for a camera’s data source.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
class HMCameraSource
```

## Topics

### Getting the properties

var aspectRatio: Double

The aspect ratio of the camera.

### Initializers

init()Deprecated

## Relationships

### Inherits From

- NSObject

### Inherited By

- HMCameraSnapshot
- HMCameraStream

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Creating a camera view

init(source: HMCameraSource)

Creates a new camera view using the given source.

