

- Core Motion
- CMMotionManager
-  magnetometerData 

Instance Property

# magnetometerData

The latest sample of magnetometer data.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+watchOS 2.0+

``` source
var magnetometerData: CMMagnetometerData? { get }
```

## Discussion

If no magnetometer data is available, the value of this property is `nil`. An app that is receiving magnetometer data after calling startMagnetometerUpdates() periodically checks the value of this property and processes the magnetometer data.

## See Also

### Managing Magnetometer Updates

var magnetometerUpdateInterval: TimeInterval

The interval, in seconds, at which the system delivers magnetometer data to the block handler.

func startMagnetometerUpdates(to: OperationQueue, withHandler: CMMagnetometerHandler)

Starts magnetometer updates on an operation queue and with a specified handler.

func startMagnetometerUpdates()

Starts magnetometer updates without a block handler.

func stopMagnetometerUpdates()

Stops magnetometer updates.

typealias CMMagnetometerHandler

The type of block callback for handling magnetometer data.

