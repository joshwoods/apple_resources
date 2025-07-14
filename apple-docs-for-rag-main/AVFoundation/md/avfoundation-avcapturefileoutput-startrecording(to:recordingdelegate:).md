

- AVFoundation
- AVCaptureFileOutput
-  startRecording(to:recordingDelegate:) 

Instance Method

# startRecording(to:recordingDelegate:)

Starts recording media to the specified output URL.

iOS 4.0+iPadOS 4.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+

``` source
func startRecording(
    to outputFileURL: URL,
    recordingDelegate delegate: any AVCaptureFileOutputRecordingDelegate
)
```

## Parameters 

`outputFileURL`  

An object specifying the output file URL.

This method raises an invalidArgumentException if the argument isn’t a valid file URL.

`delegate`  

A delegate object that’s notified of changes to the recording state.

## Discussion

A failure occurs if you attempt to record to a URL where a file exists. To overwrite the content, delete the old file before calling this method.

In macOS, calling this method from within the captureOutput(_:didOutput:from:) method guarantees that the first samples written to the new file are those passed to the delegate method.

When you stop recording by calling stopRecording(), by changing files using this method, or because of an error, the framework writes any remaining file data in the background. Therefore, for the system to notify you upon completion, you must adopt the fileOutput(_:didFinishRecordingTo:from:error:) delegate method. The recording delegate can also optionally implement methods that inform it when the output object starts writing data, when it pauses or resumes recording, and when it’s about to finish recording.

In macOS, you don’t need to call stopRecording() before calling this method while another recording is in progress. If you call this method while the output object is recording, the framework preserves media samples between the old file and the new file. In iOS, to avoid any errors, you must call stopRecording() before calling this method again.

Note

Don’t call this method when capturing audio using AVCaptureAudioFileOutput. Use the startRecording(to:outputFileType:recordingDelegate:) method instead.

## See Also

### Starting, Stopping, Pausing, and Resuming Playback

func stopRecording()

Tells the receiver to stop recording to the current file.

func pauseRecording()

Pauses recording to the current output file.

func resumeRecording()

Resumes recording to the current output file after it was previously paused using pauseRecording().

