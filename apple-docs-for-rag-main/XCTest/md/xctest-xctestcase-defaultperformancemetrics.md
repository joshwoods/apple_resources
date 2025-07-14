

- XCTest
- XCTestCase
-  defaultPerformanceMetrics 

Type Property

# defaultPerformanceMetrics

An array of default performance metrics the test records.

``` source
class var defaultPerformanceMetrics: [XCTPerformanceMetric] { get }
```

## Discussion

When you call measure(_:), the test uses this property to determine which performance metrics to record. The default is an array that contains wallClockTime. Subclasses of XCTestCase can override this method to change the behavior of measure(_:).

## See Also

### Related Documentation

static let wallClockTime: XCTPerformanceMetric

A performance metric that records the time in seconds to execute a block of code.

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

func stopMeasuring()

Ends recording performance metrics within a block of code.

class var defaultMetrics: [any XCTMetric]

An array of default metrics the test uses to record performance.

class var defaultMeasureOptions: XCTMeasureOptions

The default measurement options the test uses to record performance.

struct XCTPerformanceMetric

Performance metrics that the test records.

