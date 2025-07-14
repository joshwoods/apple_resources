

- ReplayKit
- RPScreenRecorder
-  startRecording(handler:) 

Instance Method

# startRecording(handler:)

Starts recording the app display.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 11.0+tvOS 10.0+visionOS 1.0+

``` source
func startRecording(handler: (((any Error)?) -> Void)? = nil)
```

## Parameters 

`handler`  

A block that is called when the request completes.

`error`  
If an error occurred, this parameter holds an object that explains the error. Otherwise, the value of this parameter is `nil`. See RPRecordingErrorCode for a list of error codes specific to ReplayKit.

## Discussion

Call startRecording(handler:) on an instance of the recorder to begin recording. When startRecording(handler:) is first called, an alert window appears asking the user to confirm recording. This alert window is also presented if it has been longer than 8 minutes since the last time startRecording(handler:) was called.

## See Also

### Controlling App Recording

func stopRecording(handler: ((RPPreviewViewController?, (any Error)?) -> Void)?)

Stops the current recording.

func stopRecording(withOutput: URL, completionHandler: (((any Error)?) -> Void)?)

Stops the current recording and writes the movie to the specified output URL.

func startCapture(handler: ((CMSampleBuffer, RPSampleBufferType, (any Error)?) -> Void)?, completionHandler: (((any Error)?) -> Void)?)

Starts screen and audio capture.

enum RPSampleBufferType

The type of media clip sample being buffered.

func stopCapture(handler: (((any Error)?) -> Void)?)

Stops screen capture

func discardRecording(handler: () -> Void)

Discards the current recording.

func startRecording(withMicrophoneEnabled: Bool, handler: (((any Error)?) -> Void)?)

Starts recording the app’s audio and video.

Deprecated

