

- Distributed
-  LocalTestingInvocationDecoder 

Class

# LocalTestingInvocationDecoder

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
final class LocalTestingInvocationDecoder
```

## Topics

### Instance Methods

func decodeErrorType() throws -> (any Any.Type)?

Decode the specific error type that the distributed invocation target has recorded. Currently this effectively can only ever be `Error.self`.

func decodeGenericSubstitutions() throws -> [any Any.Type]

Decode all generic substitutions that were recorded for this invocation.

func decodeNextArgument&lt;Argument>() throws -> Argument

Attempt to decode the next argument from the underlying buffers into pre-allocated storage pointed at by ‘pointer’.

func decodeReturnType() throws -> (any Any.Type)?

Attempt to decode the known return type of the distributed invocation.

### Type Aliases

typealias SerializationRequirement

The serialization requirement that the types passed to `decodeNextArgument` are required to conform to. The type returned by `decodeReturnType` is also expected to conform to this associated type requirement.

## Relationships

### Conforms To

- DistributedTargetInvocationDecoder

## See Also

### Local Testing

class LocalTestingDistributedActorSystem

A `DistributedActorSystem` designed for local only testing.

struct LocalTestingActorID

typealias LocalTestingActorAddressDeprecated

struct LocalTestingInvocationEncoder

struct LocalTestingInvocationResultHandler

