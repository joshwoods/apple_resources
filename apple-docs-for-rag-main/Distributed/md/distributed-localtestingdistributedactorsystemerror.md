

- Distributed
-  LocalTestingDistributedActorSystemError 

Structure

# LocalTestingDistributedActorSystemError

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
struct LocalTestingDistributedActorSystemError
```

## Topics

### Initializers

init(message: String)

### Instance Properties

let message: String

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

struct ExecuteDistributedTargetError

Error thrown by executeDistributedTarget(on:target:invocationDecoder:handler:).

