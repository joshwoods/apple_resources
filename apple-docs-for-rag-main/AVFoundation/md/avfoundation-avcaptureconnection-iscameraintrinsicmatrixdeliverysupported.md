

- AVFoundation
- AVCaptureConnection
-  isCameraIntrinsicMatrixDeliverySupported 

Instance Property

# isCameraIntrinsicMatrixDeliverySupported

A Boolean value that indicates whether the capture connection currently supports delivering camera intrinsics information.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var isCameraIntrinsicMatrixDeliverySupported: Bool { get }
```

## Discussion

A value of true means you can set isCameraIntrinsicMatrixDeliveryEnabled to true. The property is only true if both the connection’s input device format and output type support delivering camera intrinsics. In iOS 11, the AVCaptureVideoDataOutput class is the only output type that supports camera intrinsics.

## See Also

### Delivering camera calibration settings

var isCameraIntrinsicMatrixDeliveryEnabled: Bool

A Boolean value that indicates whether the connection can configure the capture pipeline to deliver camera intrinsics information.

