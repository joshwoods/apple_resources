

- Combine
- Publishers
-  Publishers.Buffer 

Structure

# Publishers.Buffer

A publisher that buffers elements from an upstream publisher.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct Buffer where Upstream : Publisher
```

## Topics

### Creating a Buffer Publisher

init(upstream: Upstream, size: Int, prefetch: Publishers.PrefetchStrategy, whenFull: Publishers.BufferingStrategy&lt;Publishers.Buffer&lt;Upstream>.Failure>)

Creates a publisher that buffers elements received from an upstream publisher.

### Declaring Publisher Topography

typealias Output

The kind of values published by this publisher.

typealias Failure

The kind of errors this publisher might publish.

### Inspecting Publisher Properties

let upstream: Upstream

The publisher from which this publisher receives elements.

let size: Int

The maximum number of elements to store.

let prefetch: Publishers.PrefetchStrategy

The strategy for initially populating the buffer.

let whenFull: Publishers.BufferingStrategy&lt;Publishers.Buffer&lt;Upstream>.Failure>

The action to take when the buffer becomes full.

### Applying Operators

Publisher Operators

Methods that create downstream publishers or subscribers to act on the elements they receive.

### Default Implementations

Publisher Implementations

## Relationships

### Conforms To

- Publisher

## See Also

### Buffering Elements

enum BufferingStrategy

A strategy that handles exhaustion of a buffer’s capacity.

enum PrefetchStrategy

A strategy for filling a buffer.

