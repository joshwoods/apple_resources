

- Core Motion
- CMBatchedSensorManager
-  CMBatchedSensorManager.AccelerometerUpdates 

Structure

# CMBatchedSensorManager.AccelerometerUpdates

watchOS 10.0+

``` source
struct AccelerometerUpdates
```

## Topics

### Structures

struct Iterator

## Relationships

### Conforms To

- AsyncSequence

## See Also

### Collecting accelerometer data

func startAccelerometerUpdates()

func startAccelerometerUpdates(handler: ([CMAccelerometerData]?, (any Error)?) -> Void)

func stopAccelerometerUpdates()

var accelerometerBatch: [CMAccelerometerData]?

func accelerometerUpdates() -> CMBatchedSensorManager.AccelerometerUpdates

var isAccelerometerActive: Bool

