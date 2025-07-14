

- XCTest
- XCTestCase
-  measure(metrics:block:) 

Instance Method

# measure(metrics:block:)

Records the selected metrics for a block of code.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+tvOS 13.0+visionOS 1.0+watchOS 7.0+

``` source
func measure(
    metrics: [any XCTMetric],
    block: () -> Void
)
```

## Parameters 

`metrics`  

An array of metrics to measure, like CPU, memory, or elapsed time.

`block`  

A block whose performance is measured.

## See Also

### Measuring Performance

func measure(() -> Void)

Measures the performance of a block of code.

func measureMetrics([XCTPerformanceMetric], automaticallyStartMeasuring: Bool, for: () -> Void)

Measures the performance of a block of code, optionally deferring the starting point for measurement.

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

