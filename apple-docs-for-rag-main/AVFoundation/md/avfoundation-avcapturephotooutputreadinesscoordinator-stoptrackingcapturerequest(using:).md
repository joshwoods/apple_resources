

- AVFoundation
- AVCapturePhotoOutputReadinessCoordinator
-  stopTrackingCaptureRequest(using:) 

Instance Method

# stopTrackingCaptureRequest(using:)

Stop tracking the capture request represented by the specified photo setting’s unique identifier.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+

``` source
func stopTrackingCaptureRequest(using settingsUniqueID: Int64)
```

## Parameters 

`settingsUniqueID`  

The uniqueID value of the related photo settings object.

## See Also

### Performing tracking requests

func startTrackingCaptureRequest(using: AVCapturePhotoSettings)

Tracks a capture request that uses the specified photo settings.

