

- Foundation
- Operation
-  isAsynchronous 

Instance Property

# isAsynchronous

A Boolean value indicating whether the operation executes its task asynchronously.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var isAsynchronous: Bool { get }
```

## Discussion

The value of this property is true for operations that run asynchronously with respect to the current thread or false for operations that run synchronously on the current thread. The default value of this property is false.

When implementing an asynchronous operation object, you must implement this property and return true. For more information about how to implement an asynchronous operation, see Asynchronous Versus Synchronous Operations.

## See Also

### Getting the Operation Status

var isCancelled: Bool

A Boolean value indicating whether the operation has been cancelled

var isExecuting: Bool

A Boolean value indicating whether the operation is currently executing.

var isFinished: Bool

A Boolean value indicating whether the operation has finished executing its task.

var isConcurrent: Bool

A Boolean value indicating whether the operation executes its task asynchronously.

var isReady: Bool

A Boolean value indicating whether the operation can be performed now.

var name: String?

The name of the operation.

