

- Foundation
- OperationQueue
-  addOperation(\_:) 

Instance Method

# addOperation(\_:)

Adds the specified operation to the receiver.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func addOperation(_ op: Operation)
```

## Parameters 

`op`  

The operation to be added to the queue.

## Discussion

Once added, the specified operation remains in the queue until it finishes executing.

Important

An operation object can be in at most one operation queue at a time and this method throws an invalidArgumentException exception if the operation is already in another queue. Similarly, this method throws an invalidArgumentException exception if the operation is currently executing or has already finished executing.

## See Also

### Related Documentation

func cancel()

Advises the operation object that it should stop executing its task.

var isExecuting: Bool

A Boolean value indicating whether the operation is currently executing.

### Managing Operations in the Queue

func addOperations([Operation], waitUntilFinished: Bool)

Adds the specified operations to the queue.

func addOperation(() -> Void)

Wraps the specified block in an operation and adds it to the receiver.

func addBarrierBlock(() -> Void)

Invokes a block when the queue finishes all enqueued operations, and prevents subsequent operations from starting until the block has completed.

func cancelAllOperations()

Cancels all queued and executing operations.

func waitUntilAllOperationsAreFinished()

Blocks the current thread until all the receiver’s queued and executing operations finish executing.

var operations: [Operation]

The operations currently in the queue.

Deprecated

var operationCount: Int

The number of operations currently in the queue.

Deprecated

