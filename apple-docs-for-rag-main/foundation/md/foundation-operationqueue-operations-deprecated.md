

- Foundation
- OperationQueue
-  operations Deprecated

Instance Property

# operations

The operations currently in the queue.

iOS 2.0–18.4DeprecatediPadOS 2.0–18.4DeprecatedMac Catalyst 13.1+macOS 10.5–15.4DeprecatedtvOS 9.0–18.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 2.0–9.0Deprecated

``` source
var operations: [Operation] { get }
```

Deprecated

To avoid race conditions while accessing operations, use addBarrierBlock(_:) instead.

## Discussion

The array in this property contains zero or more Operation objects in the order you added them to the queue. This order doesn’t necessarily reflect the order in which the queue invokes those operations.

You can use this property to access the operations queued at any given moment. Operations remain queued until they finish their task. Therefore, the array may contain operations that are currently running or waiting to run. The list may also contain operations that were running when you retrieved the array but have subsequently finished.

You can monitor changes to the value of this property using Key-value observing (KVO). Configure an observer to monitor the operations key path of the operation queue.

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

var operationCount: Int

The number of operations currently in the queue.

Deprecated

