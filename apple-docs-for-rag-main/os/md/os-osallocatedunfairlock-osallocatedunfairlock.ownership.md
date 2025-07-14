

- os
- OSAllocatedUnfairLock
-  OSAllocatedUnfairLock.Ownership 

Enumeration

# OSAllocatedUnfairLock.Ownership

An enumeration that represents the ownership status of an unfair lock.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
@frozen
enum Ownership
```

## Topics

### Specifying ownership

case owner

Describes code that owns the lock.

case notOwner

Describes code that doesn’t own the lock.

## Relationships

### Conforms To

- BitwiseCopyable
- Copyable
- Equatable
- Hashable
- Sendable

## See Also

### Determining lock ownership

func precondition(OSAllocatedUnfairLock&lt;State>.Ownership)

Asserts if the lock object fails to meet specified ownership requirements.

