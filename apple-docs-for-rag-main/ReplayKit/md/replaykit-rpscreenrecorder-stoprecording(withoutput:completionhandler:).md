

- ReplayKit
- RPScreenRecorder
-  stopRecording(withOutput:completionHandler:) 

Instance Method

# stopRecording(withOutput:completionHandler:)

Stops the current recording and writes the movie to the specified output URL.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
func stopRecording(
    withOutput url: URL,
    completionHandler: (((any Error)?) -> Void)? = nil
)
```

``` source
func stopRecording(withOutput url: URL) async throws
```

## Parameters 

`url`  

The output URL.

`completionHandler`  

The completion handler the system calls when the movie is written to the specified output URL. If an error occured, the system passes the completion handler an NSError that indicates the reason the operation failed.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func stopRecording(withOutput url: URL) async throws
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

## See Also

### Controlling App Recording

func startRecording(handler: (((any Error)?) -> Void)?)

Starts recording the app display.

func stopRecording(handler: ((RPPreviewViewController?, (any Error)?) -> Void)?)

Stops the current recording.

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

