

- ReplayKit
- RPScreenRecorder
-  startRecording(withMicrophoneEnabled:handler:) Deprecated

Instance Method

# startRecording(withMicrophoneEnabled:handler:)

Starts recording the app’s audio and video.

iOS 9.0–10.0DeprecatediPadOS 9.0–10.0DeprecatedMac Catalyst 13.1–13.1DeprecatedtvOS 9.0–10.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
func startRecording(
    withMicrophoneEnabled microphoneEnabled: Bool,
    handler: (((any Error)?) -> Void)? = nil
)
```

Deprecated

Use microphoneEnabled property

## Parameters 

`microphoneEnabled`  

Set to true to activate the microphone during the recording. Defaults to false.

`handler`  

A block that is called when the request completes.

`error`  
If an error occurred, this parameter holds an object that explains the error. Otherwise, the value of this parameter is `nil`. See RPRecordingErrorCode for a list of error codes specific to ReplayKit.

## Discussion

Call startRecording(withMicrophoneEnabled:handler:) on an instance of the recorder to begin recording. When startRecording(withMicrophoneEnabled:handler:) is first called, an alert window appears asking the user to confirm recording. This alert window is also presented if it has been longer than 8 minutes since the last time startRecording(withMicrophoneEnabled:handler:) was called.

## See Also

### Controlling App Recording

func startRecording(handler: (((any Error)?) -> Void)?)

Starts recording the app display.

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

