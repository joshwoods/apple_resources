

- ReplayKit
- RPScreenRecorder
-  isCameraEnabled 

Instance Property

# isCameraEnabled

A Boolean value that indicates whether the camera is currently enabled.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 11.0+visionOS 1.0+

``` source
var isCameraEnabled: Bool { get set }
```

## Discussion

The default value of this property is false. Set this property to true to enable the camera. When the app runs in visionOS, the value in this property is false and assigning a new value has no effect.

You can use this property for key-value observing.

Note

In your app’s `Info.plist` file, you must set the `Privacy - Camera Usage Description` key with a string that describes how your app uses the camera footage.

## See Also

### Inspecting a Screen Recorder

var isAvailable: Bool

A Boolean value that indicates whether the screen recorder is available for recording.

var isRecording: Bool

A Boolean value that indicates whether the app is currently recording.

var isMicrophoneEnabled: Bool

A Boolean value that indicates whether the microphone is currently enabled.

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

