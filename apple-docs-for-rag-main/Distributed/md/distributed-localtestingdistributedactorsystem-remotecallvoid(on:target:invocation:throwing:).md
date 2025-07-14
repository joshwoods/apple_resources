

- Distributed
- LocalTestingDistributedActorSystem
-  remoteCallVoid(on:target:invocation:throwing:) 

Instance Method

# remoteCallVoid(on:target:invocation:throwing:)

Invoked by the Swift runtime when making a remote call.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
final func remoteCallVoid(
    on actor: Act,
    target: RemoteCallTarget,
    invocation: inout LocalTestingDistributedActorSystem.InvocationEncoder,
    throwing errorType: Err.Type
) async throws where Act : DistributedActor, Err : Error, Act.ID == LocalTestingActorID
```

## Discussion

The `arguments` are the arguments container that was previously created by `makeInvocationEncoder` and has been populated with all arguments.

This method should perform the actual remote function call, and await for its response.

## Errors

This method is allowed to throw because of underlying transport or serialization errors, as well as by re-throwing the error received from the remote callee (if able to).

