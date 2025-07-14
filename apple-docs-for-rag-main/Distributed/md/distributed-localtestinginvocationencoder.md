

- Distributed
-  LocalTestingInvocationEncoder 

Structure

# LocalTestingInvocationEncoder

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
struct LocalTestingInvocationEncoder
```

## Topics

### Instance Methods

func doneRecording() throws

Invoked to signal to the encoder that no further `record...` calls will be made on it.

func recordArgument&lt;Value>(RemoteCallArgument&lt;Value>) throws

Record an argument of `Argument` type. This will be invoked for every argument of the target, in declaration order.

func recordErrorType&lt;E>(E.Type) throws

Record the error type of the distributed method. This method will not be invoked if the target is not throwing.

func recordGenericSubstitution&lt;T>(T.Type) throws

The arguments must be encoded order-preserving, and once `decodeGenericSubstitutions` is called, the substitutions must be returned in the same order in which they were recorded.

func recordReturnType&lt;R>(R.Type) throws

Record the return type of the distributed method. This method will not be invoked if the target is returning `Void`.

### Type Aliases

typealias SerializationRequirement

The serialization requirement that the types passed to `recordArgument` and `recordReturnType` are required to conform to.

## Relationships

### Conforms To

- DistributedTargetInvocationEncoder

## See Also

### Local Testing

class LocalTestingDistributedActorSystem

A `DistributedActorSystem` designed for local only testing.

struct LocalTestingActorID

typealias LocalTestingActorAddressDeprecated

class LocalTestingInvocationDecoder

struct LocalTestingInvocationResultHandler

