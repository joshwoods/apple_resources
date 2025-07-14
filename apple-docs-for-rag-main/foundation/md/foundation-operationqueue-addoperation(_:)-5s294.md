

- Foundation
- OperationQueue
-  addOperation(\_:) 

Instance Method

# addOperation(\_:)

Wraps the specified block in an operation and adds it to the receiver.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func addOperation(_ block: @escaping () -> Void)
```

## Parameters 

`block`  

The block to execute from the operation. The block takes no parameters and has no return value.

## Discussion

This method adds a single block to the receiver by first wrapping it in an operation object. You should not attempt to get a reference to the newly created operation object or determine its type information.

## See Also

### Related Documentation

func cancel()

Advises the operation object that it should stop executing its task.

var isExecuting: Bool

A Boolean value indicating whether the operation is currently executing.

### Managing Operations in the Queue

func addOperation(Operation)

Adds the specified operation to the receiver.

func addOperations([Operation], waitUntilFinished: Bool)

Adds the specified operations to the queue.

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

