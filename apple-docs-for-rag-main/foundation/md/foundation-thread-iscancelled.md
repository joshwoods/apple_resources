

- Foundation
- Thread
-  isCancelled 

Instance Property

# isCancelled

A Boolean value that indicates whether the receiver is cancelled.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var isCancelled: Bool { get }
```

## Discussion

true if the receiver has been cancelled, otherwise false.

If your thread supports cancellation, it should check this property periodically and exit if it ever returns true.

## See Also

### Related Documentation

func cancel()

Changes the cancelled state of the receiver to indicate that it should exit.

### Determining the Thread’s Execution State

var isExecuting: Bool

A Boolean value that indicates whether the receiver is executing.

var isFinished: Bool

A Boolean value that indicates whether the receiver has finished execution.

