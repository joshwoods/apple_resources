

- Distributed
- DistributedActorSystem
-  remoteCallVoid(on:target:invocation:throwing:) 

Instance Method

# remoteCallVoid(on:target:invocation:throwing:)

Invoked by the Swift runtime when making a remote call.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func remoteCallVoid(
    on actor: Act,
    target: RemoteCallTarget,
    invocation: inout Self.InvocationEncoder,
    throwing: Err.Type
) async throws where Act : DistributedActor, Err : Error, Self.ActorID == Act.ID
```

**Required**

## Discussion

The `arguments` are the arguments container that was previously created by `makeInvocationEncoder` and has been populated with all arguments.

This method should perform the actual remote function call, and await for its response.

## Errors

This method is allowed to throw because of underlying transport or serialization errors, as well as by re-throwing the error received from the remote callee (if able to).

