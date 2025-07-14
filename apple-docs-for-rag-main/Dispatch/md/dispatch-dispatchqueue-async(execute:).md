

- Dispatch
- DispatchQueue
-  async(execute:) 

Instance Method

# async(execute:)

Schedules a work item for immediate execution, and returns immediately.

iOS 8.0+iPadOS 8.0+Mac CatalystmacOS 10.10+tvOSvisionOSwatchOS

``` source
func async(execute workItem: DispatchWorkItem)
```

## Parameters 

`workItem`  

The work item containing the task to execute. For information on how to create this work item, see DispatchWorkItem.

## See Also

### Executing Tasks Asynchronously

func asyncAfter(deadline: DispatchTime, execute: DispatchWorkItem)

Schedules a work item for execution at the specified time, and returns immediately.

func asyncAfter(deadline: DispatchTime, qos: DispatchQoS, flags: DispatchWorkItemFlags, execute: () -> Void)

Schedules a block for execution using the specified attributes, and returns immediately.

func asyncAfter(wallDeadline: DispatchWallTime, execute: DispatchWorkItem)

Schedules a work item for execution after the specified time, and returns immediately.

func asyncAfter(wallDeadline: DispatchWallTime, qos: DispatchQoS, flags: DispatchWorkItemFlags, execute: () -> Void)

Schedules a block for execution using the specified attributes, and returns immediately.

