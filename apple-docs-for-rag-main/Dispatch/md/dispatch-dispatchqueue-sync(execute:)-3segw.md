

- Dispatch
- DispatchQueue
-  sync(execute:) 

Instance Method

# sync(execute:)

Submits a block object for execution and returns after that block finishes executing.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func sync(execute block: () -> Void)
```

## Parameters 

`block`  

The block that contains the work to perform. This block has no return value and no parameters. This parameter cannot be `NULL`.

## Discussion

This function submits a block to the specified dispatch queue for synchronous execution. Unlike dispatch_async, this function does not return until the block has finished. Calling this function and targeting the current queue results in deadlock.

Unlike with dispatch_async, no retain is performed on the target queue. Because calls to this function are synchronous, it “borrows” the reference of the caller. Moreover, no `Block_copy` is performed on the block.

As a performance optimization, this function executes blocks on the current thread whenever possible, with one exception: Blocks submitted to the main dispatch queue always run on the main thread.

## See Also

### Executing Tasks Synchronously

func sync(execute: DispatchWorkItem)

Submits a work item for execution on the current queue and returns after that block finishes executing.

func sync&lt;T>(execute: () throws -> T) rethrows -> T

Submits a work item for execution and returns the results from that item after it finishes executing.

func sync&lt;T>(flags: DispatchWorkItemFlags, execute: () throws -> T) rethrows -> T

Submits a work item for execution using the specified attributes and returns the results from that item after it finishes executing.

func asyncAndWait(execute: () -> Void)

Submits a work item for execution and returns only after it finishes executing.

