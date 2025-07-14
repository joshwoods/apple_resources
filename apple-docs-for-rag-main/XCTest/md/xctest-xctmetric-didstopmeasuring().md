

- XCTest
- XCTMetric
-  didStopMeasuring() 

Instance Method

# didStopMeasuring()

A method that XCTest calls when it has finished running the measured code.

``` source
optional func didStopMeasuring()
```

## Discussion

XCTest calls this method when it has finished running the code in the performance test’s `measure()` or `measure(metrics:)` block. It calls the method once for each iteration of a performance test. Use this method to finish gathering measurements.

## See Also

### Recording Metrics

func willBeginMeasuring()

A method that XCTest calls when it’s ready to begin running the measured code.

