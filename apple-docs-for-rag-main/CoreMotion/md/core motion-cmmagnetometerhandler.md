

- Core Motion
-  CMMagnetometerHandler 

Type Alias

# CMMagnetometerHandler

The type of block callback for handling magnetometer data.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.15+watchOS 2.0+

``` source
typealias CMMagnetometerHandler = (CMMagnetometerData?, (any Error)?) -> Void
```

## Discussion

Blocks of type `CMMagnetometerHandler` are called when there is magnetometer data to process. You pass the block into the startMagnetometerUpdates(to:withHandler:) method as the second argument. Blocks of this type return no value but take two arguments:

`magnetometerData`  
An object that encapsulates a CMMagneticField structure with fields holding magnetic-field values for the three axes of movement.

`error`  
An error object representing an error encountered in providing magnetometer data. If an error occurs, you should stop magnetometer updates and inform the user of the problem. If there is no error, this argument is `nil`. Core Motion errors are of the CMErrorDomain domain and the CMError type.

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

var magnetometerData: CMMagnetometerData?

The latest sample of magnetometer data.

