

- ReplayKit
- RPScreenRecorder
-  startCapture(handler:completionHandler:) 

Instance Method

# startCapture(handler:completionHandler:)

Starts screen and audio capture.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 11.0+tvOS 11.0+visionOS 1.0+

``` source
func startCapture(
    handler captureHandler: ((CMSampleBuffer, RPSampleBufferType, (any Error)?) -> Void)?,
    completionHandler: (((any Error)?) -> Void)? = nil
)
```

``` source
func startCapture(handler captureHandler: ((CMSampleBuffer, RPSampleBufferType, (any Error)?) -> Void)?) async throws
```

## Parameters 

`captureHandler`  

A block that is called continuously during screen capture.

sampleBuffer  
A doc://com.apple.documentation/documentation/coremedia/cmsamplebuffer-u71 object containing either audio or video data.

bufferType  
An RPSampleBufferType identifying the media type of the recorded sample.

error  
Contains an error code if screen capture failed to start. Otherwise, the value of this parameter is `nil`.

`completionHandler`  

A block that is called when screen capture has started.

error  
If an error occurred, this parameter holds an object that explains the error. Otherwise, the value of this parameter is `nil`. See RPRecordingErrorCode for a list of error codes to ReplayKit.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func startCapture(handler captureHandler: ((CMSampleBuffer, RPSampleBufferType, Error?) -> Void)?) async throws
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

## See Also

### Controlling App Recording

func startRecording(handler: (((any Error)?) -> Void)?)

Starts recording the app display.

func stopRecording(handler: ((RPPreviewViewController?, (any Error)?) -> Void)?)

Stops the current recording.

func stopRecording(withOutput: URL, completionHandler: (((any Error)?) -> Void)?)

Stops the current recording and writes the movie to the specified output URL.

enum RPSampleBufferType

The type of media clip sample being buffered.

func stopCapture(handler: (((any Error)?) -> Void)?)

Stops screen capture

func discardRecording(handler: () -> Void)

Discards the current recording.

func startRecording(withMicrophoneEnabled: Bool, handler: (((any Error)?) -> Void)?)

Starts recording the app’s audio and video.

Deprecated

