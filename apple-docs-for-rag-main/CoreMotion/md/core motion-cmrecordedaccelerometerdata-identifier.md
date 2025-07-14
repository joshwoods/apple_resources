

- Core Motion
- CMRecordedAccelerometerData
-  identifier 

Instance Property

# identifier

The unique identifier for the accelerometer data.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+visionOS 1.0+watchOS 2.0+

``` source
var identifier: UInt64 { get }
```

## Discussion

Accelerometer data is recorded in batches, which are assigned a unique identifier. This property contains the identifier of the batch in which this particular sample was recorded.

## See Also

### Getting the Accelerometer Data

var startDate: Date

The wall clock time when the sensor sample was recorded.

