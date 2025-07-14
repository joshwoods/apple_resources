

- Combine
- Publishers
-  Publishers.Contains 

Structure

# Publishers.Contains

A publisher that emits a Boolean value when it receives a specific element from its upstream publisher.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct Contains where Upstream : Publisher, Upstream.Output : Equatable
```

## Topics

### Creating a Contains Publisher

init(upstream: Upstream, output: Upstream.Output)

Creates a publisher that emits a Boolean value when it receives a specific element from its upstream publisher.

### Declaring Publisher Topography

typealias Output

The kind of values published by this publisher.

typealias Failure

The kind of errors this publisher might publish.

### Inspecting Publisher Properties

let upstream: Upstream

The publisher from which this publisher receives elements.

let output: Upstream.Output

The element to match in the upstream publisher.

### Comparing Publishers

static func == (Publishers.Contains&lt;Upstream>, Publishers.Contains&lt;Upstream>) -> Bool

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

### Applying Matching Criteria to Elements

struct ContainsWhere

A publisher that emits a Boolean value upon receiving an element that satisfies the predicate closure.

struct TryContainsWhere

A publisher that emits a Boolean value upon receiving an element that satisfies the throwing predicate closure.

struct AllSatisfy

A publisher that publishes a single Boolean value that indicates whether all received elements pass a given predicate.

struct TryAllSatisfy

A publisher that publishes a single Boolean value that indicates whether all received elements pass a given error-throwing predicate.

