

- AVFoundation
- AVCaptureConnection
-  isCameraIntrinsicMatrixDeliveryEnabled 

Instance Property

# isCameraIntrinsicMatrixDeliveryEnabled

A Boolean value that indicates whether the connection can configure the capture pipeline to deliver camera intrinsics information.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var isCameraIntrinsicMatrixDeliveryEnabled: Bool { get set }
```

## Discussion

You can set this property to true for a video connection if isCameraIntrinsicMatrixDeliverySupported is true, and only before calling the AVCaptureSession startRunning() method. The default value is false.

Camera intrinsics describe the current imaging parameters of a capture device in ways that you can use to render overlays or perform computer vision tasks. If true, any AVCaptureVideoDataOutput instance in this connection can include the kCMSampleBufferAttachmentKey_CameraIntrinsicMatrix attachment for each sample buffer it vends.

## See Also

### Delivering camera calibration settings

var isCameraIntrinsicMatrixDeliverySupported: Bool

A Boolean value that indicates whether the capture connection currently supports delivering camera intrinsics information.

