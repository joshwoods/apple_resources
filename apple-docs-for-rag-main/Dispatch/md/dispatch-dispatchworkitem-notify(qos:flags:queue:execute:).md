

- Dispatch
- DispatchWorkItem
-  notify(qos:flags:queue:execute:) 

Instance Method

# notify(qos:flags:queue:execute:)

Schedules the execution of the specified work item, with the specified quality-of-service, after the completion of the current work item.

iOS 8.0+iPadOS 8.0+Mac CatalystmacOS 10.10+tvOSvisionOSwatchOS

``` source
func notify(
    qos: DispatchQoS = .unspecified,
    flags: DispatchWorkItemFlags = [],
    queue: DispatchQueue,
    execute: @escaping () -> Void
)
```

## Parameters 

`qos`  

The quality-of-service class to use when prioritizing the work item’s execution. For a list of possible values, see DispatchQoS.

`flags`  

Configuration flags for the work item. For a list of possible values, see DispatchWorkItemFlags.

`queue`  

The queue on which to execute the work item in the execute parameter.

`execute`  

The work item to execute after the completion of the current work item.

## See Also

### Adding a Completion Handler

func notify(queue: DispatchQueue, execute: DispatchWorkItem)

Schedules the execution of the specified work item after the completion of the current work item.

