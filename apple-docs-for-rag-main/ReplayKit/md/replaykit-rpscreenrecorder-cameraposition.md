

- ReplayKit
- RPScreenRecorder
-  cameraPosition 

Instance Property

# cameraPosition

The camera position to use.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 11.0+visionOS 1.0+

``` source
var cameraPosition: RPCameraPosition { get set }
```

## Discussion

The default value of this property is AVCaptureDevice.Position.front. You can use this property for key-value observing.

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

enum RPCameraPosition

The position of the camera being accessed.

var delegate: (any RPScreenRecorderDelegate)?

The delegate for the screen recorder.

protocol RPScreenRecorderDelegate

The protocol you implement to receive notifications from the screen recorder.

