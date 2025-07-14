

- Core Motion
- CMMotionManager
-  startMagnetometerUpdates() 

Instance Method

# startMagnetometerUpdates()

Starts magnetometer updates without a block handler.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+watchOS 2.0+

``` source
func startMagnetometerUpdates()
```

## Discussion

You can get the latest magnetometer data through the magnetometerData property. You must call stopMagnetometerUpdates() when you no longer want your app to process magnetometer updates.

## See Also

### Managing Magnetometer Updates

var magnetometerUpdateInterval: TimeInterval

The interval, in seconds, at which the system delivers magnetometer data to the block handler.

func startMagnetometerUpdates(to: OperationQueue, withHandler: CMMagnetometerHandler)

Starts magnetometer updates on an operation queue and with a specified handler.

func stopMagnetometerUpdates()

Stops magnetometer updates.

var magnetometerData: CMMagnetometerData?

The latest sample of magnetometer data.

typealias CMMagnetometerHandler

The type of block callback for handling magnetometer data.

