

- Foundation
- OperationQueue
-  current 

Type Property

# current

Returns the operation queue that launched the current operation.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class var current: OperationQueue? { get }
```

## Return Value

The operation queue that started the operation or `nil` if the queue could not be determined.

## Discussion

You can use this method from within a running operation object to get a reference to the operation queue that started it. Calling this method from outside the context of a running operation typically results in `nil` being returned.

## See Also

### Related Documentation

Concurrency Programming Guide

### Accessing Specific Operation Queues

class var main: OperationQueue

Returns the operation queue associated with the main thread.

