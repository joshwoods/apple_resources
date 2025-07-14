

- AVFAudio
- AVAudioRecorder
-  record(atTime:forDuration:) 

Instance Method

# record(atTime:forDuration:)

Records audio starting at a specific time for the indicated duration.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.9+tvOS 17.0+visionOS 1.0+watchOS 4.0+

``` source
func record(
    atTime time: TimeInterval,
    forDuration duration: TimeInterval
) -> Bool
```

## Parameters 

`time`  

The time at which to start recording, relative to deviceCurrentTime.

`duration`  

The duration of time to record, in seconds.

## Return Value

true if recording was successful; otherwise, false.

## Discussion

The recorder automatically stops recording when it reaches the indicated duration. You may also use it to synchronize recording of multiple recorders as shown below.

```
func startSynchronizedRecording() {
    // Create a start time relative to the current device time.
    let time = recorderOne.deviceCurrentTime + 0.01
    let duration: TimeInterval = 10.0

    // Synchronize recording of both recorders.
    recorderOne.record(atTime: time, forDuration: duration)
    recorderTwo.record(atTime: time, forDuration: duration)
}
```

Calling this method implicitly calls prepareToRecord(), which creates an audio file and prepares the system for recording.

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

func pause()

Pauses an audio recording.

func stop()

Stops recording and closes the audio file.

var isRecording: Bool

A Boolean value that indicates whether the audio recorder is recording.

func deleteRecording() -> Bool

Deletes a recorded audio file.

