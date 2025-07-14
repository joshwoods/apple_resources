

- Distributed
- LocalTestingDistributedActorSystem
-  DistributedActorSystem Implementations 

API Collection

# DistributedActorSystem Implementations

## Topics

### Instance Methods

func executeDistributedTarget&lt;Act>(on: Act, target: RemoteCallTarget, invocationDecoder: inout Self.InvocationDecoder, handler: Self.ResultHandler) async throws

Prepare and execute a call to the distributed function identified by the passed arguments, on the passed `actor`, and collect its results using the `ResultHandler`.

