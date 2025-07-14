

- AVFoundation
- AVCaptureFileOutput
-  pauseRecording() 

Instance Method

# pauseRecording()

Pauses recording to the current output file.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 10.7+tvOS 18.0+

``` source
func pauseRecording()
```

## Discussion

This method causes the receiver to stop writing captured samples to the current output file returned by outputFileURL, but leaves the file open so that samples can be written to it in the future, if resumeRecording() is called. This allows you to record multiple media segments that are not contiguous in time to a single file.

In macOS, if this method is called within the captureOutput:didOutputSampleBuffer:fromConnection: delegate method, the last samples written to the current file are guaranteed to be those that were output immediately before those in the sample buffer passed to that method.

## See Also

### Related Documentation

var isRecordingPaused: Bool

Indicates whether recording to the current output file is paused.

### Starting, Stopping, Pausing, and Resuming Playback

func startRecording(to: URL, recordingDelegate: any AVCaptureFileOutputRecordingDelegate)

Starts recording media to the specified output URL.

func stopRecording()

Tells the receiver to stop recording to the current file.

func resumeRecording()

Resumes recording to the current output file after it was previously paused using pauseRecording().

