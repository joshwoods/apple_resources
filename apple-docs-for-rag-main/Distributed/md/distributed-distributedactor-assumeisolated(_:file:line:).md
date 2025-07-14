

- Distributed
- DistributedActor
-  assumeIsolated(\_:file:line:) 

Instance Method

# assumeIsolated(\_:file:line:)

Assume that the current task is executing on this (local) distributed actor’s serial executor, or stop program execution otherwise.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
nonisolated
func assumeIsolated(
    _ operation: (isolated Self) throws -> T,
    file: StaticString = #fileID,
    line: UInt = #line
) rethrows -> T where T : Sendable
```

## Parameters 

`operation`  

The operation that will be executed if the current context is executing on the actors serial executor, and the actor is a local reference.

`file`  

The file name to print if the assertion fails. The default is where this method was called.

`line`  

The line number to print if the assertion fails The default is where this method was called.

## Return Value

The return value of the `operation`

## Discussion

This method allows to *assume and verify* that the currently executing synchronous function is actually executing on the serial executor of the this (local) distributed actor.

If that is the case, the operation is invoked isolated to the main actor (`@MainActor () -> T`), allowing synchronous access to actor local state without hopping through asynchronous boundaries.

If the current context is not running on the actor’s serial executor, this method will crash with a fatal error (similar to `preconditionIsolated()`).

This method can only be used from synchronous functions, as asynchronous functions should instead perform a normal method call to the actor, which will hop task execution to the target actor if necessary.

Note

This check is performed against the actor’s serial executor, meaning that / if another actor uses the same serial executor–by using another actor’s executor as its own unownedExecutor –this check will succeed , as from a concurrency safety perspective, the serial executor guarantees mutual exclusion of those two actors.

Throws

Rethrows the `Error` thrown by the operation if it threw

