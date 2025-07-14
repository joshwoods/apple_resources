

- Distributed
-  DistributedTargetInvocationResultHandler 

Protocol

# DistributedTargetInvocationResultHandler

Protocol a distributed invocation execution’s result handler.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
protocol DistributedTargetInvocationResultHandler
```

## Overview

An instance conforming to this type must be passed when invoking `executeDistributedTarget(on:target:invocationDecoder:handler:)` while handling an incoming distributed call.

The handler will then be invoked with the return value (or error) that the invoked target returned (or threw).

## Topics

### Associated Types

associatedtype SerializationRequirement

The serialization requirement that the value passed to `onReturn` is required to conform to.

**Required**

### Instance Methods

func onReturn&lt;Success>(value: Success) async throws

Invoked when the distributed target execution returns successfully. The `value` is the return value of the executed distributed invocation target.

**Required**

func onReturnVoid() async throws

Invoked when the distributed target execution of a `Void` returning function has completed successfully.

**Required**

func onThrow&lt;Err>(error: Err) async throws

Invoked when the distributed target execution of a target has thrown an error.

**Required**

## Relationships

### Conforming Types

- LocalTestingInvocationResultHandler

## See Also

### Remote Calls

struct RemoteCallTarget

Represents a ‘target’ of a distributed call, such as a `distributed func` or `distributed` computed property. Identification schemes may vary between systems, and are subject to evolution.

struct RemoteCallArgument

Represents an argument passed to a distributed call target.

protocol DistributedTargetInvocationEncoder

Used to encode an invocation of a distributed target (method or computed property).

protocol DistributedTargetInvocationDecoder

Decoder that must be provided to `executeDistributedTarget` and is used by the Swift runtime to decode arguments of the invocation.

