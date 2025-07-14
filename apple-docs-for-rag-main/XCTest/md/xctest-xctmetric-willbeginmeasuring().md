

- XCTest
- XCTMetric
-  willBeginMeasuring() 

Instance Method

# willBeginMeasuring()

A method that XCTest calls when it’s ready to begin running the measured code.

``` source
optional func willBeginMeasuring()
```

## Discussion

XCTest calls this method before it runs a test’s `measure()` or `measure(metrics:)` block. It calls the method once for each iteration of a performance test. Use this method to start gathering measurements.

## See Also

### Recording Metrics

func didStopMeasuring()

A method that XCTest calls when it has finished running the measured code.

