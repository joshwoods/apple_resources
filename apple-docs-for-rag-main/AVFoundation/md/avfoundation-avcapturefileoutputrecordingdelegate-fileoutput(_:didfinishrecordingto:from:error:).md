

- AVFoundation
- AVCaptureFileOutputRecordingDelegate
-  fileOutput(\_:didFinishRecordingTo:from:error:) 

Instance Method

# fileOutput(\_:didFinishRecordingTo:from:error:)

Informs the delegate when all pending data has been written to an output file.

iOS 4.0+iPadOS 4.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+

``` source
func fileOutput(
    _ output: AVCaptureFileOutput,
    didFinishRecordingTo outputFileURL: URL,
    from connections: [AVCaptureConnection],
    error: (any Error)?
)
```

**Required**

## Parameters 

`output`  

The capture file output that has finished writing the file.

`outputFileURL`  

The file URL of the file that is being written.

`connections`  

An array of AVCaptureConnection objects attached to the file output that provided the data that is being written to the file.

`error`  

If the file was not written successfully, an error object that describes the problem; otherwise `nil`.

## Discussion

This method is called whenever a file is finished. If the file was forced to be finished due to an error, the error is described in the error parameter—otherwise, the error parameter is `nil`.

This method is called when the file output has finished writing all data to a file whose recording was stopped, either because startRecording(to:recordingDelegate:) or stopRecording() were called, or because an error (described by the error parameter) occurred (if no error occurred, the error parameter is `nil`).

This method is always called for each recording request, even if no data is successfully written to the file.

You should not assume that this method will be called on a specific thread.

## See Also

### Delegate Methods

func fileOutput(AVCaptureFileOutput, didStartRecordingTo: URL, from: [AVCaptureConnection])

Informs the delegate when the output has started writing to a file.

func fileOutput(AVCaptureFileOutput, willFinishRecordingTo: URL, from: [AVCaptureConnection], error: (any Error)?)

Informs the delegate when the output will stop writing new samples to a file.

func fileOutput(AVCaptureFileOutput, didPauseRecordingTo: URL, from: [AVCaptureConnection])

Called whenever the output is recording to a file and successfully pauses the recording at the request of a client.

func fileOutput(AVCaptureFileOutput, didResumeRecordingTo: URL, from: [AVCaptureConnection])

Called whenever the output, at the request of the client, successfully resumes a file recording that was paused.

