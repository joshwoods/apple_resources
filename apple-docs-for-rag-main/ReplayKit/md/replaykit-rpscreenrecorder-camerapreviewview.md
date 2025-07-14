

- ReplayKit
- RPScreenRecorder
-  cameraPreviewView 

Instance Property

# cameraPreviewView

A view containing the contents of the front-facing camera.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 11.0+visionOS 1.0+

**macOS**

``` source
var cameraPreviewView: NSView? { get }
```

**iOS, iPadOS, Mac Catalyst, visionOS**

``` source
var cameraPreviewView: UIView? { get }
```

## Discussion

When the value in the isCameraEnabled property is true, this property contains a view with the live camera view. If the camera isn’t enabled, the value in this property is `nil`. When the app runs in visionOS, the value in this property is `nil`.

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

var cameraPosition: RPCameraPosition

The camera position to use.

enum RPCameraPosition

The position of the camera being accessed.

var delegate: (any RPScreenRecorderDelegate)?

The delegate for the screen recorder.

protocol RPScreenRecorderDelegate

The protocol you implement to receive notifications from the screen recorder.

