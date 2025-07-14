

- Foundation
- Thread
-  qualityOfService 

Instance Property

# qualityOfService

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var qualityOfService: QualityOfService { get set }
```

## See Also

### Prioritizing Thread Work

enum QualityOfService

Constants that indicate the nature and importance of work to the system.

class func threadPriority() -> Double

Returns the current thread’s priority.

var threadPriority: Double

The receiver’s priority

class func setThreadPriority(Double) -> Bool

Sets the current thread’s priority.

