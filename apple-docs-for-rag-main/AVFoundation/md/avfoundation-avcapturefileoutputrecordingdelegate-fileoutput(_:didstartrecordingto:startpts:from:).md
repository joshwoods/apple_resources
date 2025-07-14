

- AVFoundation
- AVCaptureFileOutputRecordingDelegate
-  fileOutput(\_:didStartRecordingTo:startPTS:from:) 

Instance Method

# fileOutput(\_:didStartRecordingTo:startPTS:from:)

iOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+macOS 15.2+tvOS 18.2+

``` source
optional func fileOutput(
    _ output: AVCaptureFileOutput,
    didStartRecordingTo fileURL: URL,
    startPTS: CMTime,
    from connections: [AVCaptureConnection]
)
```

## Parameters 

`output`  

The capture file output that started writing the file.

`fileURL`  

The file URL of the file that is being written.

`startPTS`  

The timestamp of the first buffer written to the file, synced with AVCaptureSession.synchronizationClock

`connections`  

An array of AVCaptureConnection objects attached to the file output that provided the data that is being written to the file.

## Discussion

```
Informs the delegate when the output has started writing to a file.
```

This method is called when the file output has started writing data to a file. If an error condition prevents any data from being written, this method may not be called. captureOutput:willFinishRecordingToOutputFileAtURL:fromConnections:error: and captureOutput:didFinishRecordingToOutputFileAtURL:fromConnections:error: will always be called, even if no data is written.

```
If this method is implemented, the alternative delegate callback -captureOutput:didStartRecordingToOutputFileAtURL:fromConnections will not be called.

Clients should not assume that this method will be called on a specific thread, and should also try to make this method as efficient as possible.
```

