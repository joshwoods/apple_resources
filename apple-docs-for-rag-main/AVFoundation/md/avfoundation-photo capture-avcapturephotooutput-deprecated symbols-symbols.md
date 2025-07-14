

- AVFoundation
- Photo capture
- AVCapturePhotoOutput
-  Deprecated Symbols 

API Collection

# Deprecated Symbols

Review unsupported symbols and their replacements.

## Topics

### Getting Formatted Output

class func jpegPhotoDataRepresentation(forJPEGSampleBuffer: CMSampleBuffer, previewPhotoSampleBuffer: CMSampleBuffer?) -> Data?

Returns data in JPEG format corresponding to the captured photo in the specified sample buffer.

Deprecated

class func dngPhotoDataRepresentation(forRawSampleBuffer: CMSampleBuffer, previewPhotoSampleBuffer: CMSampleBuffer?) -> Data?

Returns data in digital negative (DNG) format corresponding to the captured RAW photo in the specified sample buffer.

Deprecated

### Configuring Dual Camera Capture

var isDualCameraFusionSupported: Bool

A Boolean value indicating whether the capture output currently supports automatically combining image data on a dual camera device.

Deprecated

var isDualCameraDualPhotoDeliverySupported: Bool

A Boolean value indicating whether the capture output currently supports simultaneous photo capture with both cameras on a dual-camera device.

Deprecated

var isDualCameraDualPhotoDeliveryEnabled: Bool

A Boolean value that specifies whether to configure the capture pipeline for simultaneous photo capture with both cameras on a dual-camera device.

Deprecated

### Configuring High-Resolution Still Capture

var isHighResolutionCaptureEnabled: Bool

A Boolean value that specifies whether to configure the capture pipeline for high resolution still image capture.

Deprecated

### Monitoring the Visible Scene

var isStillImageStabilizationScene: Bool

A Boolean value indicating whether the scene currently being previewed by the camera warrants image stabilization.

Deprecated

### Determining Available Settings

var isStillImageStabilizationSupported: Bool

A Boolean value indicating whether the capture output currently supports automatic stabilization for still image capture.

Deprecated

