

- AVFoundation
- AVCapturePhotoOutputReadinessCoordinator
-  captureReadiness 

Instance Property

# captureReadiness

A value that indicates whether the coordinator’s photo output is ready to respond to new capture requests in a timely manner.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+

``` source
var captureReadiness: AVCapturePhotoOutput.CaptureReadiness { get }
```

## Discussion

The value incorporates the photo output’s captureReadiness property value and any requests registered by calling the startTrackingCaptureRequest(using:) method. The system updates this value before calling the readinessCoordinator(_:captureReadinessDidChange:) method.

This property is key-value observable.

