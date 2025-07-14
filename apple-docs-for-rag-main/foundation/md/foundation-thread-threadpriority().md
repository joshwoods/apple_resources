

- Foundation
- Thread
-  threadPriority() 

Type Method

# threadPriority()

Returns the current thread’s priority.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func threadPriority() -> Double
```

## Return Value

The current thread’s priority, which is specified by a floating point number from 0.0 to 1.0, where 1.0 is highest priority.

## Discussion

The priorities in this range are mapped to the operating system’s priority values. A “typical” thread priority might be 0.5, but because the priority is determined by the kernel, there is no guarantee what this value actually will be.

## See Also

### Prioritizing Thread Work

var qualityOfService: QualityOfService

enum QualityOfService

Constants that indicate the nature and importance of work to the system.

var threadPriority: Double

The receiver’s priority

class func setThreadPriority(Double) -> Bool

Sets the current thread’s priority.

