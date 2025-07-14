

- XCTest
-  XCTCPUMetric 

Class

# XCTCPUMetric

A metric to record information about CPU activity during a performance test.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+tvOS 13.0+visionOS 1.0+watchOS 7.0+

``` source
class XCTCPUMetric
```

## Overview

`XCTCPUMetric` captures the following statistics about CPU activity; each metric is captured while the block argument to a measure(metrics:block:) call runs in a performance test:

- *CPU time* is the length of time, in seconds, that the CPU is active and executing instructions for the measured target. When the CPU switches context to execute a different process or thread or becomes idle, this value doesn’t increase.

- *CPU cycles* is the number of clock cycles that occur while the CPU is active and executing instructions for the measured target.

- *CPU instructions retired* is the number of processor instructions that run to completion during execution of the measured target. It’s possible for a CPU to abandon processing an instruction during execution, for example, if the instruction is evaluated out of order and logically follows a branch in the code that the CPU discovers it doesn’t need to take. An abandoned instruction doesn’t contribute to the retired instructions metric.

## Topics

### Initializers

init()

Creates a CPU metric that records data for the current process.

init(application: XCUIApplication)

Creates a CPU metric that records data for the requested app.

init(limitingToCurrentThread: Bool)

Creates a CPU metric that optionally records data only for the current thread.

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

