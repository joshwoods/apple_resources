

- Combine
- Publishers
-  Publishers.TryDropWhile 

Structure

# Publishers.TryDropWhile

A publisher that omits elements from an upstream publisher until a given error-throwing closure returns false.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct TryDropWhile where Upstream : Publisher
```

## Topics

### Creating a Try Drop While Publisher

init(upstream: Upstream, predicate: (Publishers.TryDropWhile&lt;Upstream>.Output) throws -> Bool)

Creates a publisher that omits elements from an upstream publisher until a given error-throwing closure returns false.

### Declaring Publisher Topography

typealias Output

The kind of values published by this publisher.

typealias Failure

The kind of errors this publisher might publish.

### Inspecting Publisher Properties

let upstream: Upstream

The publisher from which this publisher receives elements.

let predicate: (Publishers.TryDropWhile&lt;Upstream>.Output) throws -> Bool

The error-throwing closure that indicates whether to drop the element.

### Applying Operators

Publisher Operators

Methods that create downstream publishers or subscribers to act on the elements they receive.

### Default Implementations

Publisher Implementations

## Relationships

### Conforms To

- Publisher

## See Also

### Applying Sequence Operations to Elements

struct DropUntilOutput

A publisher that ignores elements from the upstream publisher until it receives an element from second publisher.

struct Drop

A publisher that omits a specified number of elements before republishing later elements.

struct DropWhile

A publisher that omits elements from an upstream publisher until a given closure returns false.

struct Concatenate

A publisher that emits all of one publisher’s elements before those from another publisher.

struct PrefixWhile

A publisher that republishes elements while a predicate closure indicates publishing should continue.

struct TryPrefixWhile

A publisher that republishes elements while an error-throwing predicate closure indicates publishing should continue.

struct PrefixUntilOutput

A publisher that republishes elements until another publisher emits an element.

