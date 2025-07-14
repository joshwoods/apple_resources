

- Distributed
-  RemoteCallTarget 

Structure

# RemoteCallTarget

Represents a ‘target’ of a distributed call, such as a `distributed func` or `distributed` computed property. Identification schemes may vary between systems, and are subject to evolution.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
struct RemoteCallTarget
```

## Overview

Actor systems generally should treat the `identifier` as an opaque string, and pass it along to the remote system for in their `remoteCall` implementation. Alternative approaches are possible, where the identifiers are either compressed, cached, or represented in other ways, as long as the recipient system is able to determine which target was intended to be invoked.

The string representation will attempt to pretty print the target identifier, however its exact format is not specified and may change in future versions.

## Topics

### Operators

static func == (RemoteCallTarget, RemoteCallTarget) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Initializers

init(String)

### Instance Properties

var description: String

Attempts to pretty format the underlying target identifier. If unable to, returns the raw underlying identifier.

var hashValue: Int

The hash value.

var identifier: String

The underlying identifier of the target, returned as-is.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- CustomStringConvertible
- Equatable
- Hashable

## See Also

### Remote Calls

struct RemoteCallArgument

Represents an argument passed to a distributed call target.

protocol DistributedTargetInvocationEncoder

Used to encode an invocation of a distributed target (method or computed property).

protocol DistributedTargetInvocationDecoder

Decoder that must be provided to `executeDistributedTarget` and is used by the Swift runtime to decode arguments of the invocation.

protocol DistributedTargetInvocationResultHandler

Protocol a distributed invocation execution’s result handler.

