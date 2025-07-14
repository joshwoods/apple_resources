

- XCTest
-  XCTMemoryMetric 

Class

# XCTMemoryMetric

A metric to record the physical memory that a performance test uses.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+tvOS 13.0+visionOS 1.0+watchOS 7.0+

``` source
class XCTMemoryMetric
```

## Overview

`XCTMemoryMetric` compares the memory use before and after running the block argument to measure(metrics:block:), and reports the difference.

## Topics

### Initializers

init()

Initializes a metric that measures memory use in the current process.

init(application: XCUIApplication)

Initializes a metric that measures memory use in the target app.

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

class XCTClockMetric

A metric to record the time that elapses during a performance test.

class XCTOSSignpostMetric

A metric to record the time that a performance test spends executing a signposted region of code.

class XCTStorageMetric

A metric to record the amount of data that a performance test logically writes to storage.

class XCTApplicationLaunchMetric

A metric to record the application launch duration for a performance test.

