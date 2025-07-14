

- Core Motion
- CMBatchedSensorManager
-  startDeviceMotionUpdates(handler:) 

Instance Method

# startDeviceMotionUpdates(handler:)

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.0+visionOS 1.0+watchOS 10.0+

``` source
func startDeviceMotionUpdates(handler: @escaping ([CMDeviceMotion]?, (any Error)?) -> Void)
```

## See Also

### Collecting device-motion data

func startDeviceMotionUpdates()

func stopDeviceMotionUpdates()

var deviceMotionBatch: [CMDeviceMotion]?

func deviceMotionUpdates() -> CMBatchedSensorManager.DeviceMotionUpdates

struct DeviceMotionUpdates

var isDeviceMotionActive: Bool

