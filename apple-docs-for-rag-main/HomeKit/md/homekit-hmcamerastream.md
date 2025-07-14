

- HomeKit
-  HMCameraStream 

Class

# HMCameraStream

An object that represents a camera’s audiovisual stream.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
class HMCameraStream
```

## Topics

### Configuring the audio stream

var audioStreamSetting: HMCameraAudioStreamSetting

The stream’s current audio setting.

func updateAudioStreamSetting(HMCameraAudioStreamSetting, completionHandler: ((any Error)?) -> Void)

Updates an audio stream’s settings.

func setAudioStreamSetting(HMCameraAudioStreamSetting)Deprecated

enum HMCameraAudioStreamSetting

The options associated with a camera’s audio stream.

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

### Controlling the stream

func startStream()

Starts the camera stream.

func stopStream()

Stops the camera stream.

var cameraStream: HMCameraStream?

The current camera stream.

var streamState: HMCameraStreamState

The current state of the camera stream.

enum HMCameraStreamState

The states associated with a camera stream.

