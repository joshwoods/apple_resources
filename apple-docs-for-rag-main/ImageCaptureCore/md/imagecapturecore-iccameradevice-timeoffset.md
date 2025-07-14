

- ImageCaptureCore
- ICCameraDevice
-  timeOffset 

Instance Property

# timeOffset

The time offset, in seconds, between the camera’s clock and the computer’s clock.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.4+visionOS 1.0+

``` source
var timeOffset: TimeInterval { get }
```

## Discussion

The value of this property is positive if the camera’s clock is ahead of the computer’s clock. Ignore this property if the camera’s capabilities do not include cameraDeviceCanSyncClock.

## See Also

### Synchronizing the Clock

func requestSyncClock()

Synchronizes the camera’s clock with the computer’s clock.

