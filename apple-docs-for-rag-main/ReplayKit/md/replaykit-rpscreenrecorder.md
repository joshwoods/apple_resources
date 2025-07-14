

- ReplayKit
-  RPScreenRecorder 

Class

# RPScreenRecorder

The shared recorder object that provides the ability to record audio and video of your app.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 11.0+tvOS 10.0+visionOS 1.0+

``` source
class RPScreenRecorder
```

## Overview

Apps on a user’s device can share the recording function, with each app having its own instance of `RPScreenRecorder`. Your app can record the audio and video inside of the app, along with user commentary through the microphone. You get a reference to the recorder through the shared() function and use it to implement start-and-stop recording functionality. You can present a user interface (view controller) where a user can trim and preview recordings, and share them with other users. Only one app at a time can use the recorder on the user’s device. Your app can’t record video from AVPlayer.

## Topics

### Accessing the Shared Recorder

class func shared() -> RPScreenRecorder

Returns an app’s instance of the shared screen recorder.

### Inspecting a Screen Recorder

var isAvailable: Bool

A Boolean value that indicates whether the screen recorder is available for recording.

var isRecording: Bool

A Boolean value that indicates whether the app is currently recording.

var isMicrophoneEnabled: Bool

A Boolean value that indicates whether the microphone is currently enabled.

var isCameraEnabled: Bool

A Boolean value that indicates whether the camera is currently enabled.

var cameraPreviewView: UIView?

A view containing the contents of the front-facing camera.

var cameraPosition: RPCameraPosition

The camera position to use.

enum RPCameraPosition

The position of the camera being accessed.

var delegate: (any RPScreenRecorderDelegate)?

The delegate for the screen recorder.

protocol RPScreenRecorderDelegate

The protocol you implement to receive notifications from the screen recorder.

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

func startRecording(withMicrophoneEnabled: Bool, handler: (((any Error)?) -> Void)?)

Starts recording the app’s audio and video.

Deprecated

### Performing Clip Recording

func startClipBuffering(completionHandler: (((any Error)?) -> Void)?)

Starts buffering a clip recording.

func stopClipBuffering(completionHandler: (((any Error)?) -> Void)?)

Stops buffering a clip recording.

func exportClip(to: URL, duration: TimeInterval, completionHandler: (((any Error)?) -> Void)?)

Exports a clip recording to a file.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Replay Sharing

Recording and Streaming Your macOS App

Share screen recordings, or broadcast live audio and video of your app, by adding ReplayKit to your macOS apps and games.

class RPPreviewViewController

An object that displays a user interface where users preview and edit a screen recording that you create with ReplayKit.

