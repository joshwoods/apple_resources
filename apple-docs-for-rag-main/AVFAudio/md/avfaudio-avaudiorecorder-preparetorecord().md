

- AVFAudio
- AVAudioRecorder
-  prepareToRecord() 

Instance Method

# prepareToRecord()

Creates an audio file and prepares the system for recording.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.7+tvOS 17.0+visionOS 1.0+watchOS 4.0+

``` source
func prepareToRecord() -> Bool
```

## Return Value

true if successful; otherwise, false.

## Discussion

Calling this method creates an audio file at the URL you used to create the recorder. If a file already exists at that location, this method overwrites it.

Call this method to start recording as quickly as possible upon calling record().

## See Also

### Controlling recording

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

var isRecording: Bool

A Boolean value that indicates whether the audio recorder is recording.

func deleteRecording() -> Bool

Deletes a recorded audio file.

