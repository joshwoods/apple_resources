

- Create ML Components
- VideoReader
- VideoReader.CameraConfiguration
-  VideoReader.CameraConfiguration.PixelFormat 

Enumeration

# VideoReader.CameraConfiguration.PixelFormat

The camera pixel format.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
enum PixelFormat
```

## Topics

### Pixel formats

case bgra32

case yCbCr8BiPlanarFullRange420

### Operators

static func == (VideoReader.CameraConfiguration.PixelFormat, VideoReader.CameraConfiguration.PixelFormat) -> Bool

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

enum Position

The position of the camera for an iOS device.

enum Resolution

The camera resolution.

