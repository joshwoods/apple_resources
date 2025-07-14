

- Distributed
-  DistributedActorCodingError 

Structure

# DistributedActorCodingError

Error thrown by distributed actor systems while encountering encoding/decoding issues.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
struct DistributedActorCodingError
```

## Overview

Also thrown when an attempt to decode DistributedActor is made, but no DistributedActorSystem is available in the `Decoder`’s `userInfo[.actorSystemKey]`, as it is required to perform the resolve call.

## Topics

### Initializers

init(message: String)

### Instance Properties

let message: String

### Type Methods

static func missingActorSystemUserInfo&lt;Act>(Act.Type) -> DistributedActorCodingError

## Relationships

### Conforms To

- DistributedActorSystemError
- Error
- Sendable

## See Also

### Errors

protocol DistributedActorSystemError

Error protocol to which errors thrown by any `DistributedActorSystem` should conform.

struct ExecuteDistributedTargetError

Error thrown by executeDistributedTarget(on:target:invocationDecoder:handler:).

struct LocalTestingDistributedActorSystemError

