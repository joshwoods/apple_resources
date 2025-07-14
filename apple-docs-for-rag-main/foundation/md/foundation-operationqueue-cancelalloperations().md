

- Foundation
- OperationQueue
-  cancelAllOperations() 

Instance Method

# cancelAllOperations()

Cancels all queued and executing operations.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func cancelAllOperations()
```

## Discussion

This method calls the cancel() method on all operations currently in the queue.

Canceling the operations does not automatically remove them from the queue or stop those that are currently executing. For operations that are queued and waiting execution, the queue must still attempt to execute the operation before recognizing that it is canceled and moving it to the finished state. For operations that are already executing, the operation object itself must check for cancellation and stop what it is doing so that it can move to the finished state. In both cases, a finished (or canceled) operation is still given a chance to execute its completion block before it is removed from the queue.

## See Also

### Related Documentation

func cancel()

Advises the operation object that it should stop executing its task.

### Managing Operations in the Queue

func addOperation(Operation)

Adds the specified operation to the receiver.

func addOperations([Operation], waitUntilFinished: Bool)

Adds the specified operations to the queue.

func addOperation(() -> Void)

Wraps the specified block in an operation and adds it to the receiver.

func addBarrierBlock(() -> Void)

Invokes a block when the queue finishes all enqueued operations, and prevents subsequent operations from starting until the block has completed.

func waitUntilAllOperationsAreFinished()

Blocks the current thread until all the receiver’s queued and executing operations finish executing.

var operations: [Operation]

The operations currently in the queue.

Deprecated

var operationCount: Int

The number of operations currently in the queue.

Deprecated

