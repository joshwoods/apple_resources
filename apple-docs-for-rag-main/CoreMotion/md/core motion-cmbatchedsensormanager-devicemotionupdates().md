

- Core Motion
- CMBatchedSensorManager
-  deviceMotionUpdates() 

Instance Method

# deviceMotionUpdates()

watchOS 10.0+

``` source
func deviceMotionUpdates() -> CMBatchedSensorManager.DeviceMotionUpdates
```

## See Also

### Collecting device-motion data

func startDeviceMotionUpdates()

func startDeviceMotionUpdates(handler: ([CMDeviceMotion]?, (any Error)?) -> Void)

func stopDeviceMotionUpdates()

var deviceMotionBatch: [CMDeviceMotion]?

struct DeviceMotionUpdates

var isDeviceMotionActive: Bool

