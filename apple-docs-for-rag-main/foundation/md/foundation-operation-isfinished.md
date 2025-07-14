

- Foundation
- Operation
-  isFinished 

Instance Property

# isFinished

A Boolean value indicating whether the operation has finished executing its task.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var isFinished: Bool { get }
```

## Discussion

The value of this property is true if the operation has finished its main task or false if it is executing that task or has not yet started it.

When implementing a concurrent operation object, you must override the implementation of this property so that you can return the finished state of your operation. In your custom implementation, you must generate KVO notifications for the `isFinished` key path whenever the finished state of your operation object changes. For more information about manually generating KVO notifications, see Key-Value Observing Programming Guide.

You do not need to reimplement this property for nonconcurrent operations.

## See Also

### Getting the Operation Status

var isCancelled: Bool

A Boolean value indicating whether the operation has been cancelled

var isExecuting: Bool

A Boolean value indicating whether the operation is currently executing.

var isConcurrent: Bool

A Boolean value indicating whether the operation executes its task asynchronously.

var isAsynchronous: Bool

A Boolean value indicating whether the operation executes its task asynchronously.

var isReady: Bool

A Boolean value indicating whether the operation can be performed now.

var name: String?

The name of the operation.

