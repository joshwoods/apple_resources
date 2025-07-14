

- Core Motion
- CMBatchedSensorManager
-  stopDeviceMotionUpdates() 

Instance Method

# stopDeviceMotionUpdates()

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.0+visionOS 1.0+watchOS 10.0+

``` source
func stopDeviceMotionUpdates()
```

## See Also

### Collecting device-motion data

func startDeviceMotionUpdates()

func startDeviceMotionUpdates(handler: ([CMDeviceMotion]?, (any Error)?) -> Void)

var deviceMotionBatch: [CMDeviceMotion]?

func deviceMotionUpdates() -> CMBatchedSensorManager.DeviceMotionUpdates

struct DeviceMotionUpdates

var isDeviceMotionActive: Bool

