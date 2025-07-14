

- AVFoundation
- AVCapturePhotoOutputReadinessCoordinatorDelegate
-  readinessCoordinator(\_:captureReadinessDidChange:) 

Instance Method

# readinessCoordinator(\_:captureReadinessDidChange:)

Tells the delegate that the capture readiness state of a photo output changed.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+

``` source
optional func readinessCoordinator(
    _ coordinator: AVCapturePhotoOutputReadinessCoordinator,
    captureReadinessDidChange captureReadiness: AVCapturePhotoOutput.CaptureReadiness
)
```

## Parameters 

`coordinator`  

The delegate’s coordinator object.

`captureReadiness`  

An updated capture readiness value.

## Discussion

The system always performs this call on the main queue, so you can use it to update your user interface’s shutter button availability and appearance.

