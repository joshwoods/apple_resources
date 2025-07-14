

- Combine
- Publishers
-  Publishers.Output 

Structure

# Publishers.Output

A publisher that publishes elements specified by a range in the sequence of published elements.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct Output where Upstream : Publisher
```

## Topics

### Creating an Output Publisher

init(upstream: Upstream, range: CountableRange&lt;Int>)

Creates a publisher that publishes elements specified by a range.

### Declaring Publisher Topography

typealias Output

The kind of values published by this publisher.

typealias Failure

The kind of errors this publisher might publish.

### Inspecting Publisher Properties

let upstream: Upstream

The publisher from which this publisher receives its elements.

let range: CountableRange&lt;Int>

The range of elements to publish.

### Comparing Publishers

static func == (Publishers.Output&lt;Upstream>, Publishers.Output&lt;Upstream>) -> Bool

Returns a Boolean value that indicates whether two publishers are equivalent.

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

### Applying Operators

Publisher Operators

Methods that create downstream publishers or subscribers to act on the elements they receive.

### Default Implementations

Equatable Implementations

Publisher Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Publisher

## See Also

### Selecting Specific Elements

struct First

A publisher that publishes the first element of a stream, then finishes.

struct FirstWhere

A publisher that only publishes the first element of a stream to satisfy a predicate closure.

struct TryFirstWhere

A publisher that only publishes the first element of a stream to satisfy a throwing predicate closure.

struct Last

A publisher that waits until after the stream finishes, and then publishes the last element of the stream.

struct LastWhere

A publisher that waits until after the stream finishes and then publishes the last element of the stream that satisfies a predicate closure.

struct TryLastWhere

A publisher that waits until after the stream finishes and then publishes the last element of the stream that satisfies an error-throwing predicate closure.

