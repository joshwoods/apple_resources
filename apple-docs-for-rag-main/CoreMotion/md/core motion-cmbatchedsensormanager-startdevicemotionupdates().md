

- Core Motion
- CMBatchedSensorManager
-  startDeviceMotionUpdates() 

Instance Method

# startDeviceMotionUpdates()

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.0+visionOS 1.0+watchOS 10.0+

``` source
func startDeviceMotionUpdates()
```

## See Also

### Collecting device-motion data

func startDeviceMotionUpdates(handler: ([CMDeviceMotion]?, (any Error)?) -> Void)

func stopDeviceMotionUpdates()

var deviceMotionBatch: [CMDeviceMotion]?

func deviceMotionUpdates() -> CMBatchedSensorManager.DeviceMotionUpdates

struct DeviceMotionUpdates

var isDeviceMotionActive: Bool

