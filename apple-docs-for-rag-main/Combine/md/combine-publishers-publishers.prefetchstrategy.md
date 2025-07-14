

- Combine
- Publishers
-  Publishers.PrefetchStrategy 

Enumeration

# Publishers.PrefetchStrategy

A strategy for filling a buffer.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
enum PrefetchStrategy
```

## Topics

### Prefetching Strategies

case byRequest

A strategy that avoids prefetching and instead performs requests on demand.

case keepFull

A strategy to fill the buffer at subscription time, and keep it full thereafter.

### Supporting Hashing

var hashValue: Int

The hash value.

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Determining Equality and Inequality

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

static func == (Publishers.PrefetchStrategy, Publishers.PrefetchStrategy) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable

## See Also

### Buffering Elements

func buffer(size: Int, prefetch: Publishers.PrefetchStrategy, whenFull: Publishers.BufferingStrategy&lt;Self.Failure>) -> Publishers.Buffer&lt;Self>

Buffers elements received from an upstream publisher.

enum BufferingStrategy

A strategy that handles exhaustion of a buffer’s capacity.

