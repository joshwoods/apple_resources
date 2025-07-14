

- Core Motion
- CMBatchedSensorManager
-  startAccelerometerUpdates() 

Instance Method

# startAccelerometerUpdates()

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.0+visionOS 1.0+watchOS 10.0+

``` source
func startAccelerometerUpdates()
```

## See Also

### Collecting accelerometer data

func startAccelerometerUpdates(handler: ([CMAccelerometerData]?, (any Error)?) -> Void)

func stopAccelerometerUpdates()

var accelerometerBatch: [CMAccelerometerData]?

func accelerometerUpdates() -> CMBatchedSensorManager.AccelerometerUpdates

struct AccelerometerUpdates

var isAccelerometerActive: Bool

