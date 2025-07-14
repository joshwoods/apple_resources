

- Dispatch
- DispatchWorkItemFlags
-  inheritQoS 

Type Property

# inheritQoS

Prefer the quality-of-service class associated with the current execution context.

iOS 8.0+iPadOS 8.0+Mac CatalystmacOS 10.10+tvOSvisionOSwatchOS

``` source
static let inheritQoS: DispatchWorkItemFlags
```

## Discussion

This flag prioritizes the quality-of-service class of the current execution context over the one associated with the block, as long as doing so does not lower the quality of service.

## See Also

### Work Item Flags

static let assignCurrentContext: DispatchWorkItemFlags

Set the attributes of the work item to match the attributes of the current execution context.

static let barrier: DispatchWorkItemFlags

Cause the work item to act as a barrier block when submitted to a concurrent queue.

static let detached: DispatchWorkItemFlags

Disassociate the work item’s attributes from the current execution context.

static let enforceQoS: DispatchWorkItemFlags

Prefer the quality-of-service class associated with the block.

static let noQoS: DispatchWorkItemFlags

Execute the work item without assigning a quality-of-service class.

