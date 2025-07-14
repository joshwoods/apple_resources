

- ReplayKit
- RPScreenRecorder
-  discardRecording(handler:) 

Instance Method

# discardRecording(handler:)

Discards the current recording.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 11.0+tvOS 10.0+visionOS 1.0+

``` source
func discardRecording(handler: @escaping () -> Void)
```

## Parameters 

`handler`  

A block that is called when the request is completed.

## Discussion

discardRecording(handler:) can only be called after the handler block in stopRecording(handler:) has been called. Use the `handler` block to do any required cleanup, including setting any `RPPreviewScreenController` references to `nil`.

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

func startRecording(withMicrophoneEnabled: Bool, handler: (((any Error)?) -> Void)?)

Starts recording the app’s audio and video.

Deprecated

