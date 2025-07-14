

- Foundation
- OperationQueue
-  operationCount Deprecated

Instance Property

# operationCount

The number of operations currently in the queue.

iOS 4.0–18.4DeprecatediPadOS 4.0–18.4DeprecatedMac Catalyst 13.1+macOS 10.6–15.4DeprecatedtvOS 9.0–18.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 2.0–9.0Deprecated

``` source
var operationCount: Int { get }
```

Deprecated

To avoid race conditions while accessing operations, use addBarrierBlock(_:) instead.

## Discussion

Because the number of operations in the queue changes as those operations finish executing, the value returned by this property reflects the instantaneous number of operations at the time the property was accessed. By the time you use the value, the actual number of operations may be different. As a result, do not use this value for object enumerations or other precise calculations.

You may monitor changes to the value of this property using Key-value observing. Configure an observer to monitor the operationCount key path of the operation queue.

## See Also

### Managing Operations in the Queue

func addOperation(Operation)

Adds the specified operation to the receiver.

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

