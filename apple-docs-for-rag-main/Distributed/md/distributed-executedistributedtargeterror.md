

- Distributed
-  ExecuteDistributedTargetError 

Structure

# ExecuteDistributedTargetError

Error thrown by executeDistributedTarget(on:target:invocationDecoder:handler:).

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
struct ExecuteDistributedTargetError
```

## Overview

Inspect the errorCode for details about the underlying reason this error was thrown.

## Topics

### Initializers

init(message: String)

init(message: String, errorCode: ExecuteDistributedTargetError.ErrorCode)

### Instance Properties

let errorCode: ExecuteDistributedTargetError.ErrorCode

let message: String

### Enumerations

enum ErrorCode

## Relationships

### Conforms To

- DistributedActorSystemError
- Error
- Sendable

## See Also

### Errors

struct DistributedActorCodingError

Error thrown by distributed actor systems while encountering encoding/decoding issues.

protocol DistributedActorSystemError

Error protocol to which errors thrown by any `DistributedActorSystem` should conform.

struct LocalTestingDistributedActorSystemError

