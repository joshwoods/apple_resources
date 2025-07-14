

- XCTest
- XCTestCase
-  defaultMeasureOptions 

Type Property

# defaultMeasureOptions

The default measurement options the test uses to record performance.

``` source
@NSCopying
class var defaultMeasureOptions: XCTMeasureOptions { get }
```

## Discussion

The default measurement options the test uses when you call measure(_:). Subclasses of XCTestCase can override this property to change the default measurement options.

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

func stopMeasuring()

Ends recording performance metrics within a block of code.

class var defaultPerformanceMetrics: [XCTPerformanceMetric]

An array of default performance metrics the test records.

class var defaultMetrics: [any XCTMetric]

An array of default metrics the test uses to record performance.

struct XCTPerformanceMetric

Performance metrics that the test records.

