

- Core Motion
- CMMotionManager
-  magnetometerUpdateInterval 

Instance Property

# magnetometerUpdateInterval

The interval, in seconds, at which the system delivers magnetometer data to the block handler.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+watchOS 2.0+

``` source
var magnetometerUpdateInterval: TimeInterval { get set }
```

## Discussion

The supplies magnetometer data to the block handler specified in startMagnetometerUpdates(to:withHandler:) at regular intervals determined by the value of this property. The interval unit are in seconds. The value of this property is capped to minimum and maximum values; the maximum value is determined by the maximum frequency supported by the hardware. If your app is sensitive to the intervals of magnetometer data, it should always check the timestamps of the delivered CMMagnetometerData instances to determine the true update interval.

## See Also

### Managing Magnetometer Updates

func startMagnetometerUpdates(to: OperationQueue, withHandler: CMMagnetometerHandler)

Starts magnetometer updates on an operation queue and with a specified handler.

func startMagnetometerUpdates()

Starts magnetometer updates without a block handler.

func stopMagnetometerUpdates()

Stops magnetometer updates.

var magnetometerData: CMMagnetometerData?

The latest sample of magnetometer data.

typealias CMMagnetometerHandler

The type of block callback for handling magnetometer data.

