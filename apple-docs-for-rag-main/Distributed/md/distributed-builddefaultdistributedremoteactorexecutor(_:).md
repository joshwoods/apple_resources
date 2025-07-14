

- Distributed
-  buildDefaultDistributedRemoteActorExecutor(\_:) 

Function

# buildDefaultDistributedRemoteActorExecutor(\_:)

Obtain the unowned `SerialExecutor` that is used by by remote distributed actor references. The executor is shared between all remote default executor remote distributed actors, and it will crash if any job is enqueued on it.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
func buildDefaultDistributedRemoteActorExecutor(_ actor: Act) -> UnownedSerialExecutor where Act : DistributedActor
```

## Discussion

It is possible to obtain the executor e.g. for logging or general debugging, however attempting to enqueue work on what might potentially be a remote actor is a programming error and therefore will crash if the actor is potentially.

If one intends to use a distributed actor’s executor to schedule work on it, one should programmatically ensure that that actor is local, e.g. using the `whenLocal` functionality of distributed actors, or by other means (e.g. “knowing that it definitely must be local”)

## See Also

### Distributed Actors

protocol DistributedActor

Common protocol to which all distributed actors conform implicitly.

protocol DistributedActorSystem

A distributed actor system underpins and implements all functionality of distributed actors.

macro Resolvable()

Enables the attached to protocol to be resolved as remote distributed actor reference.

