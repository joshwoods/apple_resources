

- Dispatch
- DispatchWorkItem
-  cancel() 

Instance Method

# cancel()

Cancels the current work item asynchronously.

iOS 8.0+iPadOS 8.0+Mac CatalystmacOS 10.10+tvOSvisionOSwatchOS

``` source
func cancel()
```

## Discussion

Cancellation causes future attempts to execute the work item to return immediately. Cancellation does not affect the execution of a work item that has already begun.

Release of any resources associated with the block object is delayed until execution of the block object is next attempted (or any execution already in progress completes).

Note

Take care to ensure that a work item does not capture any resources that require execution of the block body in order to be released, such as memory allocated with `malloc(3)` on which the block body calls `free(3)`. Such resources are leaked if the block body is never executed due to cancellation.

## See Also

### Canceling a Work Item

var isCancelled: Bool

A Boolean value indicating whether the work item has been canceled.

