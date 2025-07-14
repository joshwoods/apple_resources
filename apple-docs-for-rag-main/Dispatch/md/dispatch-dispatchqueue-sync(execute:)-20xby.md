

- Dispatch
- DispatchQueue
-  sync(execute:) 

Instance Method

# sync(execute:)

Submits a work item for execution and returns the results from that item after it finishes executing.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func sync(execute work: () throws -> T) rethrows -> T
```

## Parameters 

`work`  

The work item containing the work to perform. The block encapsulated by the work item should return a result, which is then returned by this method. For information on how to create this work item, see DispatchWorkItem.

## Return Value

The return value of the item in the `work` parameter.

## See Also

### Executing Tasks Synchronously

func sync(execute: DispatchWorkItem)

Submits a work item for execution on the current queue and returns after that block finishes executing.

func sync(execute: () -> Void)

Submits a block object for execution and returns after that block finishes executing.

func sync&lt;T>(flags: DispatchWorkItemFlags, execute: () throws -> T) rethrows -> T

Submits a work item for execution using the specified attributes and returns the results from that item after it finishes executing.

func asyncAndWait(execute: () -> Void)

Submits a work item for execution and returns only after it finishes executing.

