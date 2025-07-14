

- XCTest
- XCTestCase
-  measure(\_:) 

Instance Method

# measure(\_:)

Measures the performance of a block of code.

``` source
func measure(_ block: () -> Void)
```

## Parameters 

`block`  

A block whose performance is measured.

## Discussion

Call this method from within a test method to measure the performance of a block of code. By default, this method measures the number of seconds the block of code takes to execute. Override defaultPerformanceMetrics to change the default metrics measured by this method.

Note

This method starts and stops performance measurement automatically. Use measureMetrics(_:automaticallyStartMeasuring:for:) if you need more control over when performance measurement starts and ends.

## See Also

### Measuring Performance

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

