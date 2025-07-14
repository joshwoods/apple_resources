

- Distributed
-  DistributedActorSystemError 

Protocol

# DistributedActorSystemError

Error protocol to which errors thrown by any `DistributedActorSystem` should conform.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
protocol DistributedActorSystemError : Error
```

## Relationships

### Inherits From

- Error
- Sendable

### Conforming Types

- DistributedActorCodingError
- ExecuteDistributedTargetError
- LocalTestingDistributedActorSystemError

## See Also

### Errors

struct DistributedActorCodingError

Error thrown by distributed actor systems while encountering encoding/decoding issues.

struct ExecuteDistributedTargetError

Error thrown by executeDistributedTarget(on:target:invocationDecoder:handler:).

struct LocalTestingDistributedActorSystemError

