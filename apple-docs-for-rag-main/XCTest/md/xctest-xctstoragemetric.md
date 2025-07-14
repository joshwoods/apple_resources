

- XCTest
-  XCTStorageMetric 

Class

# XCTStorageMetric

A metric to record the amount of data that a performance test logically writes to storage.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+tvOS 13.0+visionOS 1.0+watchOS 7.0+

``` source
class XCTStorageMetric
```

## Overview

`XCTStorageMetric` records the amount of data logically written to the disk in the block argument to measure(metrics:block:). The logical size of data written is the number of bytes in all requests to write to the disk. The logical size can be different from the size of physically written data, based on how the file system organizes data, and the fact that the disk controller replaces content in fixed-size blocks.

## Topics

### Initializers

init()

Creates a metric for measuring disk use in a process.

init(application: XCUIApplication)

Creates a metric for measuring disk use in the requested app.

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

class XCTMemoryMetric

A metric to record the physical memory that a performance test uses.

class XCTOSSignpostMetric

A metric to record the time that a performance test spends executing a signposted region of code.

class XCTApplicationLaunchMetric

A metric to record the application launch duration for a performance test.

