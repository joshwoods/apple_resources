

- Dispatch
- DispatchWorkItemFlags
-  barrier 

Type Property

# barrier

Cause the work item to act as a barrier block when submitted to a concurrent queue.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
static let barrier: DispatchWorkItemFlags
```

## Discussion

When submitted to a concurrent queue, a work item with this flag acts as a barrier. Work items submitted prior to the barrier execute to completion, at which point the barrier work item executes. Once the barrier work item finishes, the queue returns to scheduling work items that were submitted after the barrier.

## See Also

### Work Item Flags

static let assignCurrentContext: DispatchWorkItemFlags

Set the attributes of the work item to match the attributes of the current execution context.

static let detached: DispatchWorkItemFlags

Disassociate the work item’s attributes from the current execution context.

static let enforceQoS: DispatchWorkItemFlags

Prefer the quality-of-service class associated with the block.

static let inheritQoS: DispatchWorkItemFlags

Prefer the quality-of-service class associated with the current execution context.

static let noQoS: DispatchWorkItemFlags

Execute the work item without assigning a quality-of-service class.

