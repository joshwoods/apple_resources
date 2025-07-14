

- Dispatch
- DispatchGroup
-  notify(qos:flags:queue:execute:) 

Instance Method

# notify(qos:flags:queue:execute:)

Schedules the submission of a block with the specified attributes to a queue when all tasks in the current group have finished executing.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func notify(
    qos: DispatchQoS = .unspecified,
    flags: DispatchWorkItemFlags = [],
    queue: DispatchQueue,
    execute work: @escaping () -> Void
)
```

## Parameters 

`qos`  

The quality of service class for the work to be performed.

`flags`  

Options for how the work is performed.

For possible values, see DispatchWorkItemFlags.

`queue`  

The queue to which the supplied block is submitted when the group completes.

`work`  

The work to be performed on the dispatch queue when the group is completed.

## Discussion

This function schedules a notification block to be submitted to the specified queue when all blocks associated with the dispatch group have completed. If the group is empty (no block objects are associated with the dispatch group), the notification block object is submitted immediately. When the notification block is submitted, the group is empty.

## See Also

### Adding a Completion Handler

func notify(queue: DispatchQueue, work: DispatchWorkItem)

Schedules the submission of a block to a queue when all tasks in the current group have finished executing.

