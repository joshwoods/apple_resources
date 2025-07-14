

- Core Motion
- CMBatchedSensorManager
-  startAccelerometerUpdates(handler:) 

Instance Method

# startAccelerometerUpdates(handler:)

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.0+visionOS 1.0+watchOS 10.0+

``` source
func startAccelerometerUpdates(handler: @escaping ([CMAccelerometerData]?, (any Error)?) -> Void)
```

## See Also

### Collecting accelerometer data

func startAccelerometerUpdates()

func stopAccelerometerUpdates()

var accelerometerBatch: [CMAccelerometerData]?

func accelerometerUpdates() -> CMBatchedSensorManager.AccelerometerUpdates

struct AccelerometerUpdates

var isAccelerometerActive: Bool

