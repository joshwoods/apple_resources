

- Foundation
- Operation
-  isConcurrent 

Instance Property

# isConcurrent

A Boolean value indicating whether the operation executes its task asynchronously.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var isConcurrent: Bool { get }
```

## Discussion

Use the isAsynchronous property instead.

The value of this property is true for operations that run asynchronously with respect to the current thread or false for operations that run synchronously on the current thread. The default value of this property is false.

In macOS 10.6 and later, operation queues ignore the value in this property and always start operations on a separate thread.

## See Also

### Getting the Operation Status

var isCancelled: Bool

A Boolean value indicating whether the operation has been cancelled

var isExecuting: Bool

A Boolean value indicating whether the operation is currently executing.

var isFinished: Bool

A Boolean value indicating whether the operation has finished executing its task.

var isAsynchronous: Bool

A Boolean value indicating whether the operation executes its task asynchronously.

var isReady: Bool

A Boolean value indicating whether the operation can be performed now.

var name: String?

The name of the operation.

