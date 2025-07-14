

- AVFoundation
- AVCapturePhotoOutputReadinessCoordinator
-  startTrackingCaptureRequest(using:) 

Instance Method

# startTrackingCaptureRequest(using:)

Tracks a capture request that uses the specified photo settings.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+

``` source
func startTrackingCaptureRequest(using settings: AVCapturePhotoSettings)
```

## Parameters 

`settings`  

A settings object that the system passes capturePhoto(with:delegate:) for this capture request.

## See Also

### Performing tracking requests

func stopTrackingCaptureRequest(using: Int64)

Stop tracking the capture request represented by the specified photo setting’s unique identifier.

