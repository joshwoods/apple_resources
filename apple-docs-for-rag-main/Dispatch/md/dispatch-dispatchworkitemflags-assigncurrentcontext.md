

- Dispatch
- DispatchWorkItemFlags
-  assignCurrentContext 

Type Property

# assignCurrentContext

Set the attributes of the work item to match the attributes of the current execution context.

iOS 8.0+iPadOS 8.0+Mac CatalystmacOS 10.10+tvOSvisionOSwatchOS

``` source
static let assignCurrentContext: DispatchWorkItemFlags
```

## Discussion

When this flag is set, the work item inherits attributes such as the quality-of-service class from the dispatch queue or thread responsible for executing the task.

## See Also

### Work Item Flags

static let barrier: DispatchWorkItemFlags

Cause the work item to act as a barrier block when submitted to a concurrent queue.

static let detached: DispatchWorkItemFlags

Disassociate the work item’s attributes from the current execution context.

static let enforceQoS: DispatchWorkItemFlags

Prefer the quality-of-service class associated with the block.

static let inheritQoS: DispatchWorkItemFlags

Prefer the quality-of-service class associated with the current execution context.

static let noQoS: DispatchWorkItemFlags

Execute the work item without assigning a quality-of-service class.

