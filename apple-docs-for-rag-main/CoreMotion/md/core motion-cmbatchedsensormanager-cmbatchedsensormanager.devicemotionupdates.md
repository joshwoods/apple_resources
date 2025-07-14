

- Core Motion
- CMBatchedSensorManager
-  CMBatchedSensorManager.DeviceMotionUpdates 

Structure

# CMBatchedSensorManager.DeviceMotionUpdates

watchOS 10.0+

``` source
struct DeviceMotionUpdates
```

## Topics

### Structures

struct Iterator

## Relationships

### Conforms To

- AsyncSequence

## See Also

### Collecting device-motion data

func startDeviceMotionUpdates()

func startDeviceMotionUpdates(handler: ([CMDeviceMotion]?, (any Error)?) -> Void)

func stopDeviceMotionUpdates()

var deviceMotionBatch: [CMDeviceMotion]?

func deviceMotionUpdates() -> CMBatchedSensorManager.DeviceMotionUpdates

var isDeviceMotionActive: Bool

