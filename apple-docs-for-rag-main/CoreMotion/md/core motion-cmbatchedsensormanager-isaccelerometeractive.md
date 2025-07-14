

- Core Motion
- CMBatchedSensorManager
-  isAccelerometerActive 

Instance Property

# isAccelerometerActive

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.0+visionOS 1.0+watchOS 10.0+

``` source
var isAccelerometerActive: Bool { get }
```

## See Also

### Collecting accelerometer data

func startAccelerometerUpdates()

func startAccelerometerUpdates(handler: ([CMAccelerometerData]?, (any Error)?) -> Void)

func stopAccelerometerUpdates()

var accelerometerBatch: [CMAccelerometerData]?

func accelerometerUpdates() -> CMBatchedSensorManager.AccelerometerUpdates

struct AccelerometerUpdates

