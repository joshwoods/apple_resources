

- Create ML Components
- VideoReader
- VideoReader.CameraAsyncBuffers
-  captureSession 

Instance Property

# captureSession

The capture session.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
var captureSession: AVCaptureSession { get }
```

## Discussion

You can use the capture session to create a preview with AVCaptureVideoPreviewLayer and to configure the input device, for example switching the input camera.

```
let sequence = try await VideoReader.readCamera(configuration: configuration)
sequence.captureSession.beginConfiguration()
sequence.captureSession.removeInput(captureSession.inputs[0])
try sequence.captureSession.addInput(AVCaptureDeviceInput(device: camera))
sequence.captureSession.commitConfiguration()
```

