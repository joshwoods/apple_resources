

- Foundation
- Thread
-  setThreadPriority(\_:) 

Type Method

# setThreadPriority(\_:)

Sets the current thread’s priority.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func setThreadPriority(_ p: Double) -> Bool
```

## Parameters 

`p`  

The new priority, specified with a floating point number from 0.0 to 1.0, where 1.0 is highest priority.

## Return Value

true if the priority assignment succeeded, false otherwise.

## Discussion

The priorities in this range are mapped to the operating system’s priority values.

## See Also

### Prioritizing Thread Work

var qualityOfService: QualityOfService

enum QualityOfService

Constants that indicate the nature and importance of work to the system.

class func threadPriority() -> Double

Returns the current thread’s priority.

var threadPriority: Double

The receiver’s priority

