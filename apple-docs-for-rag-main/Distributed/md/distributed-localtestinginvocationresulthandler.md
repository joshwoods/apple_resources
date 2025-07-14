

- Distributed
-  LocalTestingInvocationResultHandler 

Structure

# LocalTestingInvocationResultHandler

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
struct LocalTestingInvocationResultHandler
```

## Topics

### Instance Methods

func onReturn&lt;Success>(value: Success) async throws

Invoked when the distributed target execution returns successfully. The `value` is the return value of the executed distributed invocation target.

func onReturnVoid() async throws

Invoked when the distributed target execution of a `Void` returning function has completed successfully.

func onThrow&lt;Err>(error: Err) async throws

Invoked when the distributed target execution of a target has thrown an error.

### Type Aliases

typealias SerializationRequirement

The serialization requirement that the value passed to `onReturn` is required to conform to.

## Relationships

### Conforms To

- DistributedTargetInvocationResultHandler

## See Also

### Local Testing

class LocalTestingDistributedActorSystem

A `DistributedActorSystem` designed for local only testing.

struct LocalTestingActorID

typealias LocalTestingActorAddressDeprecated

struct LocalTestingInvocationEncoder

class LocalTestingInvocationDecoder

