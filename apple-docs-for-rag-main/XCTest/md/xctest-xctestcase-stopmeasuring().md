

- XCTest
- XCTestCase
-  stopMeasuring() 

Instance Method

# stopMeasuring()

Ends recording performance metrics within a block of code.

``` source
func stopMeasuring()
```

## Discussion

Call this method to end the measurement of metrics by the measureMetrics(_:automaticallyStartMeasuring:for:) method. Measurement will end immediately after this method is called from within the measured block.

Note

You must call measureMetrics(_:automaticallyStartMeasuring:for:) with an `automaticallyStartMeasuring` value of false in order to set a custom end point with stopMeasuring().

## See Also

### Measuring Performance

func measure(() -> Void)

Measures the performance of a block of code.

func measureMetrics([XCTPerformanceMetric], automaticallyStartMeasuring: Bool, for: () -> Void)

Measures the performance of a block of code, optionally deferring the starting point for measurement.

func measure(metrics: [any XCTMetric], block: () -> Void)

Records the selected metrics for a block of code.

func measure(metrics: [any XCTMetric], options: XCTMeasureOptions, block: () -> Void)

Records the selected metrics, using the specified measurement options, for a block of code.

func measure(options: XCTMeasureOptions, block: () -> Void)

Records the performance, using the specified measurement options, for a block of code.

func startMeasuring()

Starts recording performance metrics within a block of code.

class var defaultPerformanceMetrics: [XCTPerformanceMetric]

An array of default performance metrics the test records.

class var defaultMetrics: [any XCTMetric]

An array of default metrics the test uses to record performance.

class var defaultMeasureOptions: XCTMeasureOptions

The default measurement options the test uses to record performance.

struct XCTPerformanceMetric

Performance metrics that the test records.

