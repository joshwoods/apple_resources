

- Dispatch
- DispatchQueue
-  async(group:execute:) 

Instance Method

# async(group:execute:)

Schedules a work item asynchronously for execution and associates it with the specified dispatch group.

iOS 8.0+iPadOS 8.0+Mac CatalystmacOS 10.10+tvOSvisionOSwatchOS

``` source
func async(
    group: DispatchGroup,
    execute workItem: DispatchWorkItem
)
```

## Parameters 

`group`  

The dispatch group to associate with the work item. This parameter cannot be `NULL`.

`workItem`  

The work item containing the task to execute. For information on how to create this work item, see DispatchWorkItem.

## Discussion

This method adds the work item to the group before scheduling it on the current queue.

## See Also

### Dispatching Work to Groups

func async(group: DispatchGroup?, qos: DispatchQoS, flags: DispatchWorkItemFlags, execute: () -> Void)

Schedules a block asynchronously for execution and optionally associates it with a dispatch group.

