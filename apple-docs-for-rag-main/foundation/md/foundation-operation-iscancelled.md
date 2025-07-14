

- Foundation
- Operation
-  isCancelled 

Instance Property

# isCancelled

A Boolean value indicating whether the operation has been cancelled

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var isCancelled: Bool { get }
```

## Discussion

The default value of this property is false. Calling the cancel() method of this object sets the value of this property to true. Once canceled, an operation must move to the finished state.

Canceling an operation does not actively stop the receiver’s code from executing. An operation object is responsible for calling this method periodically and stopping itself if the method returns true.

You should always check the value of this property before doing any work towards accomplishing the operation’s task, which typically means checking it at the beginning of your custom main() method. It is possible for an operation to be cancelled before it begins executing or at any time while it is executing. Therefore, checking the value at the beginning of your main() method (and periodically throughout that method) lets you exit as quickly as possible when an operation is cancelled.

## See Also

### Related Documentation

func cancel()

Advises the operation object that it should stop executing its task.

### Getting the Operation Status

var isExecuting: Bool

A Boolean value indicating whether the operation is currently executing.

var isFinished: Bool

A Boolean value indicating whether the operation has finished executing its task.

var isConcurrent: Bool

A Boolean value indicating whether the operation executes its task asynchronously.

var isAsynchronous: Bool

A Boolean value indicating whether the operation executes its task asynchronously.

var isReady: Bool

A Boolean value indicating whether the operation can be performed now.

var name: String?

The name of the operation.

