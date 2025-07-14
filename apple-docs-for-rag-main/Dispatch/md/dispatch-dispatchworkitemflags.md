

- Dispatch
-  DispatchWorkItemFlags 

Structure

# DispatchWorkItemFlags

A set of behaviors for a work item, such as its quality-of-service class and whether to create a barrier or spawn a new detached thread.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct DispatchWorkItemFlags
```

## Topics

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

static let noQoS: DispatchWorkItemFlags

Execute the work item without assigning a quality-of-service class.

## Relationships

### Conforms To

- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Creating a Work Item

init(qos: DispatchQoS, flags: DispatchWorkItemFlags, block: () -> Void)

Creates a new dispatch work item from an existing block and assigns it the specified quality-of-service class.

