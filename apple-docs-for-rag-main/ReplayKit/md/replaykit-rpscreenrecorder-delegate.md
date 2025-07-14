

- ReplayKit
- RPScreenRecorder
-  delegate 

Instance Property

# delegate

The delegate for the screen recorder.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 11.0+tvOS 10.0+visionOS 1.0+

``` source
weak var delegate: (any RPScreenRecorderDelegate)? { get set }
```

## Discussion

Set the delegate to respond to changes by the recorder; for example, when the recording stops.

## See Also

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

protocol RPScreenRecorderDelegate

The protocol you implement to receive notifications from the screen recorder.

