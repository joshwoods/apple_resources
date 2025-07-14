

- XCTest
- XCTestCase
-  measureMetrics(\_:automaticallyStartMeasuring:for:) 

Instance Method

# measureMetrics(\_:automaticallyStartMeasuring:for:)

Measures the performance of a block of code, optionally deferring the starting point for measurement.

``` source
func measureMetrics(
    _ metrics: [XCTPerformanceMetric],
    automaticallyStartMeasuring: Bool,
    for block: () -> Void
)
```

## Parameters 

`metrics`  

An array of performance metrics to measure. Each metric is measured across calls to the block. Pass wallClockTime to measure the number of seconds taken to execute the block of code.

`automaticallyStartMeasuring`  

If false, measurements will not be taken until startMeasuring() is called inside the block.

`block`  

A block whose performance is measured.

## Discussion

Call this method from within a test method to measure the performance of a block of code. This method provides more granular control over performance measurement than the measure(_:) method, and should be used when you need to customize the points at which measurement starts and ends within the block, or wish to measure multiple metrics for the block.

Performance measurement must be started and stopped exactly once within the block. As a result:

- If `automaticallyStartMeasuring` is true and startMeasuring() is called inside the block, the test will fail.

- If `automaticallyStartMeasuring` is false, startMeasuring() must be called once and only once before the end of the block, or the test will fail.

- If stopMeasuring() is called multiple times during the block the test will fail.

## See Also

### Related Documentation

static let wallClockTime: XCTPerformanceMetric

A performance metric that records the time in seconds to execute a block of code.

### Measuring Performance

func measure(() -> Void)

Measures the performance of a block of code.

func measure(metrics: [any XCTMetric], block: () -> Void)

Records the selected metrics for a block of code.

func measure(metrics: [any XCTMetric], options: XCTMeasureOptions, block: () -> Void)

Records the selected metrics, using the specified measurement options, for a block of code.

func measure(options: XCTMeasureOptions, block: () -> Void)

Records the performance, using the specified measurement options, for a block of code.

func startMeasuring()

Starts recording performance metrics within a block of code.

func stopMeasuring()

Ends recording performance metrics within a block of code.

class var defaultPerformanceMetrics: [XCTPerformanceMetric]

An array of default performance metrics the test records.

class var defaultMetrics: [any XCTMetric]

An array of default metrics the test uses to record performance.

class var defaultMeasureOptions: XCTMeasureOptions

The default measurement options the test uses to record performance.

struct XCTPerformanceMetric

Performance metrics that the test records.

