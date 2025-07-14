

- Core Motion
- CMBatchedSensorManager
-  accelerometerBatch 

Instance Property

# accelerometerBatch

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.0+visionOS 1.0+watchOS 10.0+

``` source
var accelerometerBatch: [CMAccelerometerData]? { get }
```

## See Also

### Collecting accelerometer data

func startAccelerometerUpdates()

func startAccelerometerUpdates(handler: ([CMAccelerometerData]?, (any Error)?) -> Void)

func stopAccelerometerUpdates()

func accelerometerUpdates() -> CMBatchedSensorManager.AccelerometerUpdates

struct AccelerometerUpdates

var isAccelerometerActive: Bool

