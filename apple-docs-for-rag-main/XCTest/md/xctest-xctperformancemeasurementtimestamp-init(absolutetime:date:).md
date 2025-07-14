

- XCTest
- XCTPerformanceMeasurementTimestamp
-  init(absoluteTime:date:) 

Initializer

# init(absoluteTime:date:)

Intitializes a timestamp that represents the provided time.

``` source
init(
    absoluteTime: UInt64,
    date: Date
)
```

## Parameters 

`absoluteTime`  

The time, as returned by the mach_absolute_time system call.

`date`  

The time, represented as a Date.

## See Also

### Initializers

convenience init()

Intitializes a timestamp that represents the current time.

