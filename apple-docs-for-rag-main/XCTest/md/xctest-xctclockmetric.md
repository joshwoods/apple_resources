

- XCTest
-  XCTClockMetric 

Class

# XCTClockMetric

A metric to record the time that elapses during a performance test.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+tvOS 13.0+visionOS 1.0+watchOS 7.0+

``` source
class XCTClockMetric
```

## Overview

`XCTClockMetric` measures the total elapsed time during execution of the block argument to measure(metrics:block:). The metric records time monotonically, regardless of changes to the system clock. Its result includes time spent executing code under test, and time when the CPU is idle or running other code.

## Topics

### Initializing an Item

init()

Initializes a metric that records elapsed time in a performance test.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol
- XCTMetric

## See Also

### Measurement Metrics

protocol XCTMetric

A protocol that defines the methods that objects must provide when gathering metrics during performance tests.

class XCTCPUMetric

A metric to record information about CPU activity during a performance test.

class XCTMemoryMetric

A metric to record the physical memory that a performance test uses.

class XCTOSSignpostMetric

A metric to record the time that a performance test spends executing a signposted region of code.

class XCTStorageMetric

A metric to record the amount of data that a performance test logically writes to storage.

class XCTApplicationLaunchMetric

A metric to record the application launch duration for a performance test.

