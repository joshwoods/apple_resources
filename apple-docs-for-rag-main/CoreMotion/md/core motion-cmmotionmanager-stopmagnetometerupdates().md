

- Core Motion
- CMMotionManager
-  stopMagnetometerUpdates() 

Instance Method

# stopMagnetometerUpdates()

Stops magnetometer updates.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+watchOS 2.0+

``` source
func stopMagnetometerUpdates()
```

## See Also

### Managing Magnetometer Updates

var magnetometerUpdateInterval: TimeInterval

The interval, in seconds, at which the system delivers magnetometer data to the block handler.

func startMagnetometerUpdates(to: OperationQueue, withHandler: CMMagnetometerHandler)

Starts magnetometer updates on an operation queue and with a specified handler.

func startMagnetometerUpdates()

Starts magnetometer updates without a block handler.

var magnetometerData: CMMagnetometerData?

The latest sample of magnetometer data.

typealias CMMagnetometerHandler

The type of block callback for handling magnetometer data.

