

- PHASE
-  PHASECalibrationMode 

Enumeration

# PHASECalibrationMode

Calibration options for sound pressure level.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
enum PHASECalibrationMode
```

## Topics

### Modes

case absoluteSpl

A sound pressure level based on the current output device.

case none

An option that specifies no loudness calibration.

case relativeSpl

A sound pressure level that’s tuned for the device.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Audio-Providing Nodes

class PHASESamplerNodeDefinition

A node that plays complete audio data.

enum PHASEPlaybackMode

Loop options for audio playback.

class PHASEPushStreamNodeDefinition

A node that plays a sequence of audio buffers.

class PHASEPushStreamNode

An audio stream you manage to provide a sound buffer data.

struct PHASEPushStreamBufferOptions

Options that inform PHASE of an audio-stream buffer’s playback priority.

class PHASEGeneratorNodeDefinition

A base class for nodes that provide audio data to generate sound.

