

- AVFoundation
- AVCaptureFileOutputRecordingDelegate
-  fileOutput(\_:didPauseRecordingTo:from:) 

Instance Method

# fileOutput(\_:didPauseRecordingTo:from:)

Called whenever the output is recording to a file and successfully pauses the recording at the request of a client.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 10.7+tvOS 18.0+

``` source
optional func fileOutput(
    _ output: AVCaptureFileOutput,
    didPauseRecordingTo fileURL: URL,
    from connections: [AVCaptureConnection]
)
```

## Parameters 

`output`  

The capture file output that has paused its file recording.

`fileURL`  

The file URL of the file that is being written.

`connections`  

An array of AVCaptureConnection objects attached to the file output that provided the data that is being written to the file.

## Discussion

This method is called whenever a request to pause recording is actually respected.

It is safe for delegates to change what the file output is currently doing (starting a new file, for example) from within this method. If recording to a file is stopped, either manually or due to an error, this method is not guaranteed to be called, even if a previous call to `pauseRecording` was made.

You should not assume that this method will be called on a specific thread, and should make this method as efficient as possible.

## See Also

### Delegate Methods

func fileOutput(AVCaptureFileOutput, didStartRecordingTo: URL, from: [AVCaptureConnection])

Informs the delegate when the output has started writing to a file.

func fileOutput(AVCaptureFileOutput, willFinishRecordingTo: URL, from: [AVCaptureConnection], error: (any Error)?)

Informs the delegate when the output will stop writing new samples to a file.

func fileOutput(AVCaptureFileOutput, didFinishRecordingTo: URL, from: [AVCaptureConnection], error: (any Error)?)

Informs the delegate when all pending data has been written to an output file.

**Required**

func fileOutput(AVCaptureFileOutput, didResumeRecordingTo: URL, from: [AVCaptureConnection])

Called whenever the output, at the request of the client, successfully resumes a file recording that was paused.

