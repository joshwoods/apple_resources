

- ImageCaptureCore
- ICCameraDevice
-  requestSyncClock() 

Instance Method

# requestSyncClock()

Synchronizes the camera’s clock with the computer’s clock.

macOS 10.4+

``` source
func requestSyncClock()
```

## Discussion

Send this request only if the camera has the cameraDeviceCanSyncClock capability.

## See Also

### Synchronizing the Clock

var timeOffset: TimeInterval

The time offset, in seconds, between the camera’s clock and the computer’s clock.

