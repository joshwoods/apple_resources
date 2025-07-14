

- PHASE
-  PHASEPushStreamCompletionCallbackCondition 

Enumeration

# PHASEPushStreamCompletionCallbackCondition

A status that describes the results after the app schedules a push-stream buffer.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
enum PHASEPushStreamCompletionCallbackCondition
```

## Overview

A PHASEPushStreamNode object provides an instance of this class to the completion closure after the app schedules a buffer by calling scheduleBuffer(buffer:completionCallbackType:completionHandler:).

## Topics

### Conditions

case dataRendered

Indicates the framework invokes the callback when the engine processes the audio for output.

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

### Providing Audio Data

func scheduleBuffer(buffer: AVAudioPCMBuffer)

Schedules audio data for playback.

func scheduleBuffer(buffer: AVAudioPCMBuffer, time: AVAudioTime?, options: PHASEPushStreamBufferOptions)

Schedules audio data playback at a specific time.

func scheduleBuffer(buffer: AVAudioPCMBuffer, time: AVAudioTime?, options: PHASEPushStreamBufferOptions, completionCallbackType: PHASEPushStreamCompletionCallbackCondition, completionHandler: (PHASEPushStreamCompletionCallbackCondition) -> Void)

Schedules audio data playback at a specific time with a completion handler.

func scheduleBuffer(buffer: AVAudioPCMBuffer, completionCallbackType: PHASEPushStreamCompletionCallbackCondition, completionHandler: (PHASEPushStreamCompletionCallbackCondition) -> Void)

Schedules audio data playback with a completion handler.

