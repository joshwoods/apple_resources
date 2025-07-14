

- Distributed
- DistributedActor
-  whenLocal(\_:) 

Instance Method

# whenLocal(\_:)

Executes the passed ‘body’ only when the distributed actor is local instance.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
nonisolated
func whenLocal(_ body: (isolated Self) async throws(E) -> T) async throws(E) -> T? where T : Sendable, E : Error
```

## Discussion

The `Self` passed to the body closure is isolated, meaning that the closure can be used to call non-distributed functions, or even access actor state.

When the actor is remote, the closure won’t be executed and this function will return nil.

