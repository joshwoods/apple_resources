

- Create ML Components
- VideoReader
- VideoReader.CameraConfiguration
-  VideoReader.CameraConfiguration.Resolution 

Enumeration

# VideoReader.CameraConfiguration.Resolution

The camera resolution.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
enum Resolution
```

## Topics

### Camera resolutions

case high

case low

case medium

### Operators

static func == (VideoReader.CameraConfiguration.Resolution, VideoReader.CameraConfiguration.Resolution) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- Sendable

## See Also

### Creating a camera configuration

init()

Creates a camera configuration.

init(position: VideoReader.CameraConfiguration.Position, pixelFormat: VideoReader.CameraConfiguration.PixelFormat, resolution: VideoReader.CameraConfiguration.Resolution, frameRate: Double)

Creates a camera configuration.

enum PixelFormat

The camera pixel format.

enum Position

The position of the camera for an iOS device.

