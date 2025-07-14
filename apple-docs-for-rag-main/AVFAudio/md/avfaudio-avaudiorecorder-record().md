

- AVFAudio
- AVAudioRecorder
-  record() 

Instance Method

# record()

Starts or resumes audio recording.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.7+tvOS 17.0+visionOS 1.0+watchOS 4.0+

``` source
func record() -> Bool
```

## Return Value

true if successful; otherwise, false.

## Discussion

Calling this method implicitly calls prepareToRecord(), which creates an audio file and prepares the system for recording.

## See Also

### Controlling recording

func prepareToRecord() -> Bool

Creates an audio file and prepares the system for recording.

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

var isRecording: Bool

A Boolean value that indicates whether the audio recorder is recording.

func deleteRecording() -> Bool

Deletes a recorded audio file.

