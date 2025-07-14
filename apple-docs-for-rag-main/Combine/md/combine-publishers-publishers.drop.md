

- Combine
- Publishers
-  Publishers.Drop 

Structure

# Publishers.Drop

A publisher that omits a specified number of elements before republishing later elements.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct Drop where Upstream : Publisher
```

## Topics

### Creating a Drop Publisher

init(upstream: Upstream, count: Int)

Creates a publisher that omits a specified number of elements before republishing later elements.

### Declaring Publisher Topography

typealias Output

The kind of values published by this publisher.

typealias Failure

The kind of errors this publisher might publish.

### Inspecting Publisher Properties

let upstream: Upstream

The publisher from which this publisher receives elements.

let count: Int

The number of elements to drop.

### Comparing Publishers

static func == (Publishers.Drop&lt;Upstream>, Publishers.Drop&lt;Upstream>) -> Bool

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

### Applying Sequence Operations to Elements

struct DropUntilOutput

A publisher that ignores elements from the upstream publisher until it receives an element from second publisher.

struct DropWhile

A publisher that omits elements from an upstream publisher until a given closure returns false.

struct TryDropWhile

A publisher that omits elements from an upstream publisher until a given error-throwing closure returns false.

struct Concatenate

A publisher that emits all of one publisher’s elements before those from another publisher.

struct PrefixWhile

A publisher that republishes elements while a predicate closure indicates publishing should continue.

struct TryPrefixWhile

A publisher that republishes elements while an error-throwing predicate closure indicates publishing should continue.

struct PrefixUntilOutput

A publisher that republishes elements until another publisher emits an element.

