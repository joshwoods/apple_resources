

- Combine
- Publishers
-  Publishers.Count 

Structure

# Publishers.Count

A publisher that publishes the number of elements received from the upstream publisher.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct Count where Upstream : Publisher
```

## Topics

### Creating a Count Publisher

init(upstream: Upstream)

Creates a publisher that publishes the number of elements received from the upstream publisher.

### Declaring Publisher Topography

typealias Output

The kind of values published by this publisher.

typealias Failure

The kind of errors this publisher might publish.

### Inspecting Publisher Properties

let upstream: Upstream

The publisher from which this publisher receives elements.

### Comparing Publishers

static func == (Publishers.Count&lt;Upstream>, Publishers.Count&lt;Upstream>) -> Bool

Returns a Boolean value that indicates whether two publishers are equivalent. /// - Parameters:

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

### Applying Mathematical Operations on Elements

struct Comparison

A publisher that republishes items from another publisher only if each new item is in increasing order from the previously-published item.

struct TryComparison

A publisher that republishes items from another publisher only if each new item is in increasing order from the previously-published item, and fails if the ordering logic throws an error.

