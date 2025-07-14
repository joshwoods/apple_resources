

- XCTest
-  Performance Tests 

API Collection

# Performance Tests

Gather metrics while running your code, and report a failure if the metrics become significantly worse than a baseline value.

## Topics

### Measuring Performance

Writing and running performance tests

Repeatably gather metrics on the performance of your code.

### Measurement Options

class XCTMeasureOptions

Options to control the gathering of performance measurements during tests.

### Measurement Metrics

protocol XCTMetric

A protocol that defines the methods that objects must provide when gathering metrics during performance tests.

class XCTCPUMetric

A metric to record information about CPU activity during a performance test.

class XCTClockMetric

A metric to record the time that elapses during a performance test.

class XCTMemoryMetric

A metric to record the physical memory that a performance test uses.

class XCTOSSignpostMetric

A metric to record the time that a performance test spends executing a signposted region of code.

class XCTStorageMetric

A metric to record the amount of data that a performance test logically writes to storage.

class XCTApplicationLaunchMetric

A metric to record the application launch duration for a performance test.

### Measurements

class XCTPerformanceMeasurement

A measurement from a single iteration of a performance test.

class XCTPerformanceMeasurementTimestamp

A point in time that captures the start or finish of a performance test iteration.

