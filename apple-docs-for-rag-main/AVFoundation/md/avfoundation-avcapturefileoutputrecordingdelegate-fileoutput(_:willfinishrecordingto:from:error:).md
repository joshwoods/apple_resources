

- AVFoundation
- AVCaptureFileOutputRecordingDelegate
-  fileOutput(\_:willFinishRecordingTo:from:error:) 

Instance Method

# fileOutput(\_:willFinishRecordingTo:from:error:)

Informs the delegate when the output will stop writing new samples to a file.

macOS 10.7+

``` source
optional func fileOutput(
    _ output: AVCaptureFileOutput,
    willFinishRecordingTo fileURL: URL,
    from connections: [AVCaptureConnection],
    error: (any Error)?
)
```

## Parameters 

`output`  

The capture file output that will finish writing the file.

`fileURL`  

The file URL of the file that is being written.

`connections`  

An array of AVCaptureConnection objects attached to the file output that provided the data that is being written to the file.

`error`  

An error describing what caused the file to stop recording, or `nil` if there was no error.

## Discussion

This method is called when the file output will stop recording new samples to the file at outputFileURL, either because startRecording(to:recordingDelegate:) or stopRecording() was called, or because an error (described by the error parameter) occurred (if no error occurred, the error parameter is `nil`).

This method is always called for each recording request, even if no data is successfully written to the file.

You should not assume that this method will be called on a specific thread, and should make this method as efficient as possible.

## See Also

### Delegate Methods

func fileOutput(AVCaptureFileOutput, didStartRecordingTo: URL, from: [AVCaptureConnection])

Informs the delegate when the output has started writing to a file.

func fileOutput(AVCaptureFileOutput, didFinishRecordingTo: URL, from: [AVCaptureConnection], error: (any Error)?)

Informs the delegate when all pending data has been written to an output file.

**Required**

func fileOutput(AVCaptureFileOutput, didPauseRecordingTo: URL, from: [AVCaptureConnection])

Called whenever the output is recording to a file and successfully pauses the recording at the request of a client.

func fileOutput(AVCaptureFileOutput, didResumeRecordingTo: URL, from: [AVCaptureConnection])

Called whenever the output, at the request of the client, successfully resumes a file recording that was paused.

