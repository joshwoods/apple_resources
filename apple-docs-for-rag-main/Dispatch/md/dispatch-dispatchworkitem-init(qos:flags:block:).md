

- Dispatch
- DispatchWorkItem
-  init(qos:flags:block:) 

Initializer

# init(qos:flags:block:)

Creates a new dispatch work item from an existing block and assigns it the specified quality-of-service class.

iOS 8.0+iPadOS 8.0+Mac CatalystmacOS 10.10+tvOSvisionOSwatchOS

``` source
init(
    qos: DispatchQoS = .unspecified,
    flags: DispatchWorkItemFlags = [],
    block: @escaping () -> Void
)
```

## Parameters 

`qos`  

The quality-of-service class to use when prioritizing the work item’s execution. For a list of possible values, see DispatchQoS.

`flags`  

Configuration flags for the work item. For a list of possible values, see DispatchWorkItemFlags.

`block`  

The block that performs the work.

## Discussion

Submit the returned dispatch work item to a queue to schedule it for execution in that queue. Dispatch queues may alter the specified quality-of-service level based on the specified `flags` and the quality-of-service level of the queue’s underlying threads. However, the queue never executes the block with a quality-of-service level lower than the one in the `qos` parameter.

You can also execute the dispatch work item directly in the current context by calling its perform() method. When performing a work item directly, the system never executes the block with a quality-of-service level lower than the one in the `qos` parameter.

## See Also

### Creating a Work Item

struct DispatchWorkItemFlags

A set of behaviors for a work item, such as its quality-of-service class and whether to create a barrier or spawn a new detached thread.

