

- PHASE
-  PHASEPushStreamNode 

Class

# PHASEPushStreamNode

An audio stream you manage to provide a sound buffer data.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
class PHASEPushStreamNode
```

## Overview

A sound event’s pushStreamNodes dictionary populates with an instance of this class when PHASE invokes a PHASEPushStreamNodeDefinition in your event node tree.

Your app provides the audio data that the sound event plays by calling one or more of this class’s buffer-scheduling functions, for example, scheduleBuffer(buffer:).

## Topics

### Inspecting Stream Properties

var mixer: PHASEMixer

The audio stream’s output pipeline.

var format: AVAudioFormat

The format of the audio stream data.

### Providing Audio Data

func scheduleBuffer(buffer: AVAudioPCMBuffer)

Schedules audio data for playback.

func scheduleBuffer(buffer: AVAudioPCMBuffer, time: AVAudioTime?, options: PHASEPushStreamBufferOptions)

Schedules audio data playback at a specific time.

func scheduleBuffer(buffer: AVAudioPCMBuffer, time: AVAudioTime?, options: PHASEPushStreamBufferOptions, completionCallbackType: PHASEPushStreamCompletionCallbackCondition, completionHandler: (PHASEPushStreamCompletionCallbackCondition) -> Void)

Schedules audio data playback at a specific time with a completion handler.

func scheduleBuffer(buffer: AVAudioPCMBuffer, completionCallbackType: PHASEPushStreamCompletionCallbackCondition, completionHandler: (PHASEPushStreamCompletionCallbackCondition) -> Void)

Schedules audio data playback with a completion handler.

enum PHASEPushStreamCompletionCallbackCondition

A status that describes the results after the app schedules a push-stream buffer.

### Controlling Playback

var gainMetaParameter: PHASENumberMetaParameter?

A meta parameter for dynamic loudness control.

var rateMetaParameter: PHASENumberMetaParameter?

A meta parameter for dynamic rate control.

## Relationships

### Inherits From

- PHASEStreamNode

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Audio-Providing Nodes

class PHASESamplerNodeDefinition

A node that plays complete audio data.

enum PHASEPlaybackMode

Loop options for audio playback.

class PHASEPushStreamNodeDefinition

A node that plays a sequence of audio buffers.

struct PHASEPushStreamBufferOptions

Options that inform PHASE of an audio-stream buffer’s playback priority.

enum PHASECalibrationMode

Calibration options for sound pressure level.

class PHASEGeneratorNodeDefinition

A base class for nodes that provide audio data to generate sound.

