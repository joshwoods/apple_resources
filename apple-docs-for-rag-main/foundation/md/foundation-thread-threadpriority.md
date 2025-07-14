

- Foundation
- Thread
-  threadPriority 

Instance Property

# threadPriority

The receiver’s priority

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var threadPriority: Double { get set }
```

## Discussion

The thread’s priority, which is specified by a floating point number from 0.0 to 1.0, where 1.0 is highest priority.

The priorities in this range are mapped to the operating system’s priority values. A “typical” thread priority might be 0.5, but because the priority is determined by the kernel, there is no guarantee what this value actually will be.

## See Also

### Prioritizing Thread Work

var qualityOfService: QualityOfService

enum QualityOfService

Constants that indicate the nature and importance of work to the system.

class func threadPriority() -> Double

Returns the current thread’s priority.

class func setThreadPriority(Double) -> Bool

Sets the current thread’s priority.

