

- Dispatch
- DispatchWorkItemFlags
-  noQoS 

Type Property

# noQoS

Execute the work item without assigning a quality-of-service class.

iOS 8.0+iPadOS 8.0+Mac CatalystmacOS 10.10+tvOSvisionOSwatchOS

``` source
static let noQoS: DispatchWorkItemFlags
```

## Discussion

This flag takes priority over the assignCurrentContext flag.

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

static let inheritQoS: DispatchWorkItemFlags

Prefer the quality-of-service class associated with the current execution context.

