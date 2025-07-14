

- XCTest
-  XCTMetric 

Protocol

# XCTMetric

A protocol that defines the methods that objects must provide when gathering metrics during performance tests.

``` source
protocol XCTMetric : NSCopying, NSObjectProtocol
```

## Overview

Objects that gather metrics during performance tests must conform to `XCTMetric`. Before you create your own conforming objects, first use the metrics classes that `XCTest` supplies.

## Topics

### Recording Metrics

func willBeginMeasuring()

A method that XCTest calls when it’s ready to begin running the measured code.

func didStopMeasuring()

A method that XCTest calls when it has finished running the measured code.

### Reporting Gathered Metrics

func reportMeasurements(from: XCTPerformanceMeasurementTimestamp, to: XCTPerformanceMeasurementTimestamp) throws -> [XCTPerformanceMeasurement]

Reports the measurements gathered for a metric between specific timestamps.

**Required**

## Relationships

### Inherits From

- NSCopying
- NSObjectProtocol

### Conforming Types

- XCTApplicationLaunchMetric
- XCTCPUMetric
- XCTClockMetric
- XCTMemoryMetric
- XCTOSSignpostMetric
- XCTStorageMetric

## See Also

### Measurement Metrics

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

