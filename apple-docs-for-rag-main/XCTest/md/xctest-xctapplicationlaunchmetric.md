

- XCTest
-  XCTApplicationLaunchMetric 

Class

# XCTApplicationLaunchMetric

A metric to record the application launch duration for a performance test.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+tvOS 13.0+visionOS 1.0+watchOS 7.0+

``` source
class XCTApplicationLaunchMetric
```

## Topics

### Initializers

init()

Initializes a metric that records the time for an app to display its first frame to screen and complete all extended launch tasks.

init(waitUntilResponsive: Bool)

Initializes a metric that records the time for an app to display its first frame to screen and complete all extended launch tasks, or to display its first frame and wait until the app is responsive.

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

class XCTStorageMetric

A metric to record the amount of data that a performance test logically writes to storage.

