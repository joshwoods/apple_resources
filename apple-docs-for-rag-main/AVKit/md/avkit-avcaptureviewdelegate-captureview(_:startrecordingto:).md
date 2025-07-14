

- AVKit
- AVCaptureViewDelegate
-  captureView(\_:startRecordingTo:) 

Instance Method

# captureView(\_:startRecordingTo:)

Tells the delegate that the user has made a request to start a new recording.

macOS 10.10+

``` source
func captureView(
    _ captureView: AVCaptureView,
    startRecordingTo fileOutput: AVCaptureFileOutput
)
```

**Required**

## Parameters 

`captureView`  

The capture view.

`fileOutput`  

The capture file output.

## Discussion

If the capture file output is an instance of AVCaptureMovieFileOutput, you start recording by calling startRecording(to:recordingDelegate:) on the capture file output.

