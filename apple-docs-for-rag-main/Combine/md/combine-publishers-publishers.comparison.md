

- Combine
- Publishers
-  Publishers.Comparison 

Structure

# Publishers.Comparison

A publisher that republishes items from another publisher only if each new item is in increasing order from the previously-published item.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct Comparison where Upstream : Publisher
```

## Topics

### Creating a Comparison Publisher

init(upstream: Upstream, areInIncreasingOrder: (Upstream.Output, Upstream.Output) -> Bool)

Creates a publisher that republishes items from another publisher only if each new item is in increasing order from the previously-published item.

### Declaring Publisher Topography

typealias Output

The kind of values published by this publisher.

typealias Failure

The kind of errors this publisher might publish.

### Inspecting Publisher Properties

let upstream: Upstream

The publisher from which this publisher receives its elements.

let areInIncreasingOrder: (Upstream.Output, Upstream.Output) -> Bool

A closure that receives two elements and returns true if they are in increasing order.

### Applying Operators

Publisher Operators

Methods that create downstream publishers or subscribers to act on the elements they receive.

### Default Implementations

Publisher Implementations

## Relationships

### Conforms To

- Publisher

## See Also

### Applying Mathematical Operations on Elements

struct Count

A publisher that publishes the number of elements received from the upstream publisher.

struct TryComparison

A publisher that republishes items from another publisher only if each new item is in increasing order from the previously-published item, and fails if the ordering logic throws an error.

