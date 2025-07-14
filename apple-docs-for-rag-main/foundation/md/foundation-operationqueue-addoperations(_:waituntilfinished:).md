

- Foundation
- OperationQueue
-  addOperations(\_:waitUntilFinished:) 

Instance Method

# addOperations(\_:waitUntilFinished:)

Adds the specified operations to the queue.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func addOperations(
    _ ops: [Operation],
    waitUntilFinished wait: Bool
)
```

## Parameters 

`ops`  

The operations to be added to the queue.

`wait`  

If true, the current thread is blocked until all of the specified operations finish executing. If false, the operations are added to the queue and control returns immediately to the caller.

## Discussion

An operation object can be in at most one operation queue at a time and cannot be added if it is currently executing or finished. This method throws an `NSInvalidArgumentException` exception if any of those error conditions are true for any of the operations in the `ops` parameter.

Once added, the specified `operation` remains in the queue until its isFinished method returns true.

## See Also

### Managing Operations in the Queue

func addOperation(Operation)

Adds the specified operation to the receiver.

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

