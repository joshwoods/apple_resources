

- Dispatch
- DispatchQueue
-  asyncAfter(deadline:execute:) 

Instance Method

# asyncAfter(deadline:execute:)

Schedules a work item for execution at the specified time, and returns immediately.

iOS 8.0+iPadOS 8.0+Mac CatalystmacOS 10.10+tvOSvisionOSwatchOS

``` source
func asyncAfter(
    deadline: DispatchTime,
    execute: DispatchWorkItem
)
```

## Parameters 

`deadline`  

The time at which to schedule the work item for execution. Specifying the current time is less efficient than calling the async(execute:) method directly. Do not specify the value in distantFuture; doing so is undefined.

`execute`  

The work item containing the task to execute. For information on how to create this work item, see DispatchWorkItem.

## See Also

### Executing Tasks Asynchronously

func async(execute: DispatchWorkItem)

Schedules a work item for immediate execution, and returns immediately.

func asyncAfter(deadline: DispatchTime, qos: DispatchQoS, flags: DispatchWorkItemFlags, execute: () -> Void)

Schedules a block for execution using the specified attributes, and returns immediately.

func asyncAfter(wallDeadline: DispatchWallTime, execute: DispatchWorkItem)

Schedules a work item for execution after the specified time, and returns immediately.

func asyncAfter(wallDeadline: DispatchWallTime, qos: DispatchQoS, flags: DispatchWorkItemFlags, execute: () -> Void)

Schedules a block for execution using the specified attributes, and returns immediately.

