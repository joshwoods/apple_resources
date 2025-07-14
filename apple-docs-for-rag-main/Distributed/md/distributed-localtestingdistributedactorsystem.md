

- Distributed
-  LocalTestingDistributedActorSystem 

Class

# LocalTestingDistributedActorSystem

A `DistributedActorSystem` designed for local only testing.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
final class LocalTestingDistributedActorSystem
```

## Overview

It will crash on any attempt of remote communication, but can be useful for learning about `distributed actor` isolation, as well as early prototyping stages of development where a real system is not necessary yet.

## Topics

### Initializers

init()

### Instance Methods

func actorReady&lt;Act>(Act)

Invoked during a distributed actor’s initialization, as soon as it becomes fully initialized.

func assignID&lt;Act>(Act.Type) -> LocalTestingDistributedActorSystem.ActorID

Assign an LocalTestingDistributedActorSystem.ActorID for the passed actor type.

func invokeHandlerOnReturn(handler: LocalTestingDistributedActorSystem.ResultHandler, resultBuffer: UnsafeRawPointer, metatype: any Any.Type) async throws

Implementation synthesized by the compiler. Not intended to be invoked explicitly from user code!

func makeInvocationEncoder() -> LocalTestingDistributedActorSystem.InvocationEncoder

Invoked by the Swift runtime when a distributed remote call is about to be made.

func remoteCall&lt;Act, Err, Res>(on: Act, target: RemoteCallTarget, invocation: inout LocalTestingDistributedActorSystem.InvocationEncoder, throwing: Err.Type, returning: Res.Type) async throws -> Res

Invoked by the Swift runtime when making a remote call.

func remoteCallVoid&lt;Act, Err>(on: Act, target: RemoteCallTarget, invocation: inout LocalTestingDistributedActorSystem.InvocationEncoder, throwing: Err.Type) async throws

Invoked by the Swift runtime when making a remote call.

func resignID(LocalTestingDistributedActorSystem.ActorID)

Called during when a distributed actor is deinitialized, or fails to initialize completely (e.g. by throwing out of an `init` that did not completely initialize all of the actors stored properties yet).

func resolve&lt;Act>(id: LocalTestingDistributedActorSystem.ActorID, as: Act.Type) throws -> Act?

Resolves a local or remote LocalTestingDistributedActorSystem.ActorID to a reference to given actor, or throws if unable to.

### Type Aliases

typealias ActorID

The type ID that will be assigned to any distributed actor managed by this actor system.

typealias InvocationDecoder

Type of DistributedTargetInvocationDecoder that should be used when decoding invocations during executeDistributedTarget(on:target:invocationDecoder:handler:) calls.

typealias InvocationEncoder

Type of DistributedTargetInvocationEncoder that should be used when the Swift runtime needs to encode a distributed target call into an encoder, before passing it off to `remoteCall(...)`.

typealias ResultHandler

The type of the result handler which will be offered the results returned by a distributed function invocation called via executeDistributedTarget(on:target:invocationDecoder:handler:).

typealias SerializationRequirement

The serialization requirement that will be applied to all distributed targets used with this system.

### Default Implementations

DistributedActorSystem Implementations

## Relationships

### Conforms To

- DistributedActorSystem
- Sendable

## See Also

### Local Testing

struct LocalTestingActorID

typealias LocalTestingActorAddressDeprecated

struct LocalTestingInvocationEncoder

class LocalTestingInvocationDecoder

struct LocalTestingInvocationResultHandler

