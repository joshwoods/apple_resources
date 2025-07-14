

- AVFAudio
- AVAudioRecorder
-  isRecording 

Instance Property

# isRecording

A Boolean value that indicates whether the audio recorder is recording.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.7+tvOS 17.0+visionOS 1.0+watchOS 4.0+

``` source
var isRecording: Bool { get }
```

## See Also

### Controlling recording

func prepareToRecord() -> Bool

Creates an audio file and prepares the system for recording.

func record() -> Bool

Starts or resumes audio recording.

func record(atTime: TimeInterval) -> Bool

Records audio starting at a specific time.

func record(forDuration: TimeInterval) -> Bool

Records audio for the indicated duration of time.

func record(atTime: TimeInterval, forDuration: TimeInterval) -> Bool

Records audio starting at a specific time for the indicated duration.

func pause()

Pauses an audio recording.

func stop()

Stops recording and closes the audio file.

func deleteRecording() -> Bool

Deletes a recorded audio file.

