

- ReplayKit
- RPScreenRecorder
-  isMicrophoneEnabled 

Instance Property

# isMicrophoneEnabled

A Boolean value that indicates whether the microphone is currently enabled.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 11.0+visionOS 1.0+

``` source
var isMicrophoneEnabled: Bool { get set }
```

## See Also

### Inspecting a Screen Recorder

var isAvailable: Bool

A Boolean value that indicates whether the screen recorder is available for recording.

var isRecording: Bool

A Boolean value that indicates whether the app is currently recording.

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

