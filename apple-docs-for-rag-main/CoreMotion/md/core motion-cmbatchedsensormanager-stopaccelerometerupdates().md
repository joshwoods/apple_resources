

- Core Motion
- CMBatchedSensorManager
-  stopAccelerometerUpdates() 

Instance Method

# stopAccelerometerUpdates()

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.0+visionOS 1.0+watchOS 10.0+

``` source
func stopAccelerometerUpdates()
```

## See Also

### Collecting accelerometer data

func startAccelerometerUpdates()

func startAccelerometerUpdates(handler: ([CMAccelerometerData]?, (any Error)?) -> Void)

var accelerometerBatch: [CMAccelerometerData]?

func accelerometerUpdates() -> CMBatchedSensorManager.AccelerometerUpdates

struct AccelerometerUpdates

var isAccelerometerActive: Bool

