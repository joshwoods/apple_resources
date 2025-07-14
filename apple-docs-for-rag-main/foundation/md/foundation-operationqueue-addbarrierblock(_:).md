

- Foundation
- OperationQueue
-  addBarrierBlock(\_:) 

Instance Method

# addBarrierBlock(\_:)

Invokes a block when the queue finishes all enqueued operations, and prevents subsequent operations from starting until the block has completed.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func addBarrierBlock(_ barrier: @escaping () -> Void)
```

## Parameters 

`barrier`  

The block to invoke after all currently enqueued operations have finished. Operations you add after the barrier block don’t start until the block has completed.

## Discussion

This method is similar to dispatch_barrier_async.

## See Also

### Managing Operations in the Queue

func addOperation(Operation)

Adds the specified operation to the receiver.

func addOperations([Operation], waitUntilFinished: Bool)

Adds the specified operations to the queue.

func addOperation(() -> Void)

Wraps the specified block in an operation and adds it to the receiver.

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

