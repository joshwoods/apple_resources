

- AVFAudio
-  AVAudioEngineManualRenderingMode 

Enumeration

# AVAudioEngineManualRenderingMode

The two modes for manual rendering.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
enum AVAudioEngineManualRenderingMode
```

## Overview

By default, the engine connects to an audio device and automatically renders in real time. You can configure it to operate in manual rendering mode, where it doesn’t have a connection to an audio device and renders in response to requests from the client.

## Topics

### Constants

case offline

An engine that operates in an offline mode.

case realtime

An engine that operates under real-time constraints and doesn’t make blocking calls while rendering.

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

### Constants

enum AVAudioEngineManualRenderingError

Constants that describe error codes that the framework returns from manual rendering mode methods.

enum AVAudioEngineManualRenderingStatus

Status codes that return from the render call to the engine operating in manual rendering mode.

