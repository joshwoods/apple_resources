

- Core Motion
- CMBatchedSensorManager
-  deviceMotionBatch 

Instance Property

# deviceMotionBatch

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.0+visionOS 1.0+watchOS 10.0+

``` source
var deviceMotionBatch: [CMDeviceMotion]? { get }
```

## See Also

### Collecting device-motion data

func startDeviceMotionUpdates()

func startDeviceMotionUpdates(handler: ([CMDeviceMotion]?, (any Error)?) -> Void)

func stopDeviceMotionUpdates()

func deviceMotionUpdates() -> CMBatchedSensorManager.DeviceMotionUpdates

struct DeviceMotionUpdates

var isDeviceMotionActive: Bool

