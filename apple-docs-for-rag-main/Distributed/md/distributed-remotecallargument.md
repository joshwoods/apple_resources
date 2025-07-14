

- Distributed
-  RemoteCallArgument 

Structure

# RemoteCallArgument

Represents an argument passed to a distributed call target.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
struct RemoteCallArgument
```

## Topics

### Initializers

init(label: String?, name: String, value: Value)

### Instance Properties

var effectiveLabel: String

The effective label of this argument. This reflects the semantics of call sites of function declarations without explicit label definitions in Swift.

let label: String?

The “argument label” of the argument. The label is the name visible name used in external calls made to this target, e.g. for `func hello(label name: String)` it is `label`.

let name: String

The internal name of parameter this argument is accessible as in the function body. It is not part of the functions API and may change without breaking the target identifier.

let value: Value

The value of the argument being passed to the call. As `RemoteCallArgument` is always used in conjunction with `recordArgument` and populated by the compiler, this Value will generally conform to a distributed actor system’s `SerializationRequirement`.

## See Also

### Remote Calls

struct RemoteCallTarget

Represents a ‘target’ of a distributed call, such as a `distributed func` or `distributed` computed property. Identification schemes may vary between systems, and are subject to evolution.

protocol DistributedTargetInvocationEncoder

Used to encode an invocation of a distributed target (method or computed property).

protocol DistributedTargetInvocationDecoder

Decoder that must be provided to `executeDistributedTarget` and is used by the Swift runtime to decode arguments of the invocation.

protocol DistributedTargetInvocationResultHandler

Protocol a distributed invocation execution’s result handler.

