

- Dispatch
- DispatchWorkItem
-  notify(queue:execute:) 

Instance Method

# notify(queue:execute:)

Schedules the execution of the specified work item after the completion of the current work item.

iOS 8.0+iPadOS 8.0+Mac CatalystmacOS 10.10+tvOSvisionOSwatchOS

``` source
func notify(
    queue: DispatchQueue,
    execute: DispatchWorkItem
)
```

## Parameters 

`queue`  

The queue on which to execute the work item in the `execute` parameter.

`execute`  

The work item to execute after the completion of the current work item.

## See Also

### Adding a Completion Handler

func notify(qos: DispatchQoS, flags: DispatchWorkItemFlags, queue: DispatchQueue, execute: () -> Void)

Schedules the execution of the specified work item, with the specified quality-of-service, after the completion of the current work item.

