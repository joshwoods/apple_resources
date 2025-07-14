

- Dispatch
- DispatchQueue
-  sync(execute:) 

Instance Method

# sync(execute:)

Submits a work item for execution on the current queue and returns after that block finishes executing.

iOS 8.0+iPadOS 8.0+Mac CatalystmacOS 10.10+tvOSvisionOSwatchOS

``` source
func sync(execute workItem: DispatchWorkItem)
```

## Parameters 

`workItem`  

The dispatch work item containing the task to execute. For information on how to create this work item, see DispatchWorkItem.

## See Also

### Executing Tasks Synchronously

func sync(execute: () -> Void)

Submits a block object for execution and returns after that block finishes executing.

func sync&lt;T>(execute: () throws -> T) rethrows -> T

Submits a work item for execution and returns the results from that item after it finishes executing.

func sync&lt;T>(flags: DispatchWorkItemFlags, execute: () throws -> T) rethrows -> T

Submits a work item for execution using the specified attributes and returns the results from that item after it finishes executing.

func asyncAndWait(execute: () -> Void)

Submits a work item for execution and returns only after it finishes executing.

