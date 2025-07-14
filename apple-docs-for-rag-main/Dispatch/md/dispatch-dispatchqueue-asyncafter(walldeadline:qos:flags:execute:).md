

- Dispatch
- DispatchQueue
-  asyncAfter(wallDeadline:qos:flags:execute:) 

Instance Method

# asyncAfter(wallDeadline:qos:flags:execute:)

Schedules a block for execution using the specified attributes, and returns immediately.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
@preconcurrency
func asyncAfter(
    wallDeadline: DispatchWallTime,
    qos: DispatchQoS = .unspecified,
    flags: DispatchWorkItemFlags = [],
    execute work: @escaping () -> Void
)
```

## Parameters 

`wallDeadline`  

The time at which to schedule the block for execution. Specifying the current time is less efficient than calling the async(execute:) method directly. Do not specify the value in distantFuture; doing so is undefined.

`qos`  

The quality-of-service class to use when executing the block. This parameter determines the priority with which the block is scheduled and executed. For a list of possible values, see DispatchQoS.

`flags`  

Additional attributes to apply when executing the block. For a list of possible values, see DispatchWorkItemFlags.

`work`  

The block containing the work to perform. This block has no return value and no parameters.

## See Also

### Executing Tasks Asynchronously

func async(execute: DispatchWorkItem)

Schedules a work item for immediate execution, and returns immediately.

func asyncAfter(deadline: DispatchTime, execute: DispatchWorkItem)

Schedules a work item for execution at the specified time, and returns immediately.

func asyncAfter(deadline: DispatchTime, qos: DispatchQoS, flags: DispatchWorkItemFlags, execute: () -> Void)

Schedules a block for execution using the specified attributes, and returns immediately.

func asyncAfter(wallDeadline: DispatchWallTime, execute: DispatchWorkItem)

Schedules a work item for execution after the specified time, and returns immediately.

