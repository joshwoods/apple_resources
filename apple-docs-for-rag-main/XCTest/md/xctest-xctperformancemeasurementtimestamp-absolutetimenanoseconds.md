

- XCTest
- XCTPerformanceMeasurementTimestamp
-  absoluteTimeNanoSeconds 

Instance Property

# absoluteTimeNanoSeconds

The nanoseconds component of the absolute time.

``` source
var absoluteTimeNanoSeconds: UInt64 { get }
```

## Discussion

This property reflects the number of nanoseconds since an arbitrary reference time. It doesn’t update while the system is sleeping.

## See Also

### Mach Absolute Time

var absoluteTime: UInt64

The absolute time of the timestamp, which is the value of the mach absolute time clock.

