

- XCTest
- XCTMetric
-  reportMeasurements(from:to:) 

Instance Method

# reportMeasurements(from:to:)

Reports the measurements gathered for a metric between specific timestamps.

``` source
func reportMeasurements(
    from startTime: XCTPerformanceMeasurementTimestamp,
    to endTime: XCTPerformanceMeasurementTimestamp
) throws -> [XCTPerformanceMeasurement]
```

**Required**

## Parameters 

`startTime`  

A timestamp that represents the time at which the measured code began to execute.

`endTime`  

A timestamp that represents the time at which the measured code finished executing.

## Return Value

An array of the measurements gathered by this metric during the requested interval.

## Discussion

Report the measurements gathered during the execution of measured code in a performance test. Use the `startTime` and `endTime` parameters to refine the accuracy of the reported measurements.

