

- Distributed
-  Resolvable() 

Macro

# Resolvable()

Enables the attached to protocol to be resolved as remote distributed actor reference.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
@attached(peer, names: prefixed(`$`)) @attached(extension, names: arbitrary)
macro Resolvable()
```

### Requirements

The attached to type must be a protocol that refines the `DistributedActor` protocol. It must either specify a concrete `ActorSystem` or constrain it in such way that the system’s `SerializationRequirement` is statically known.

## See Also

### Distributed Actors

protocol DistributedActor

Common protocol to which all distributed actors conform implicitly.

protocol DistributedActorSystem

A distributed actor system underpins and implements all functionality of distributed actors.

func buildDefaultDistributedRemoteActorExecutor&lt;Act>(Act) -> UnownedSerialExecutor

Obtain the unowned `SerialExecutor` that is used by by remote distributed actor references. The executor is shared between all remote default executor remote distributed actors, and it will crash if any job is enqueued on it.

