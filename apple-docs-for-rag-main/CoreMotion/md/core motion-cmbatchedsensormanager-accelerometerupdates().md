

- Core Motion
- CMBatchedSensorManager
-  accelerometerUpdates() 

Instance Method

# accelerometerUpdates()

watchOS 10.0+

``` source
func accelerometerUpdates() -> CMBatchedSensorManager.AccelerometerUpdates
```

## See Also

### Collecting accelerometer data

func startAccelerometerUpdates()

func startAccelerometerUpdates(handler: ([CMAccelerometerData]?, (any Error)?) -> Void)

func stopAccelerometerUpdates()

var accelerometerBatch: [CMAccelerometerData]?

struct AccelerometerUpdates

var isAccelerometerActive: Bool

