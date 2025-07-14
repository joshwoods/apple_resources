

- Dispatch
- DispatchGroup
-  notify(queue:work:) 

Instance Method

# notify(queue:work:)

Schedules the submission of a block to a queue when all tasks in the current group have finished executing.

iOS 8.0+iPadOS 8.0+Mac CatalystmacOS 10.10+tvOSvisionOSwatchOS

``` source
func notify(
    queue: DispatchQueue,
    work: DispatchWorkItem
)
```

## Parameters 

`queue`  

The queue to which the supplied block is submitted when the group completes.

`work`  

The work to be performed on the dispatch queue when the group is completed.

## Discussion

This function schedules a notification block to be submitted to the specified queue when all blocks associated with the dispatch group have completed. If the group is empty (no block objects are associated with the dispatch group), the notification block object is submitted immediately. When the notification block is submitted, the group is empty.

## See Also

### Adding a Completion Handler

func notify(qos: DispatchQoS, flags: DispatchWorkItemFlags, queue: DispatchQueue, execute: () -> Void)

Schedules the submission of a block with the specified attributes to a queue when all tasks in the current group have finished executing.

