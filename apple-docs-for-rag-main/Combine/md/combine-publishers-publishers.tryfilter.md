

- Combine
- Publishers
-  Publishers.TryFilter 

Structure

# Publishers.TryFilter

A publisher that republishes all elements that match a provided error-throwing closure.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct TryFilter where Upstream : Publisher
```

## Topics

### Creating a Try Filter Publisher

init(upstream: Upstream, isIncluded: (Upstream.Output) throws -> Bool)

Creates a publisher that republishes all elements that match a provided error-throwing closure.

### Declaring Publisher Topography

typealias Output

The kind of values published by this publisher.

typealias Failure

The kind of errors this publisher might publish.

### Inspecting Publisher Properties

let upstream: Upstream

The publisher from which this publisher receives elements.

let isIncluded: (Upstream.Output) throws -> Bool

An error-throwing closure that indicates whether this filter should republish an element.

### Applying Operators

Publisher Operators

Methods that create downstream publishers or subscribers to act on the elements they receive.

### Default Implementations

Publisher Implementations

## Relationships

### Conforms To

- Publisher

## See Also

### Filtering Elements

struct Filter

A publisher that republishes all elements that match a provided closure.

struct CompactMap

A publisher that republishes all non-nil results of calling a closure with each received element.

struct TryCompactMap

A publisher that republishes all non-nil results of calling an error-throwing closure with each received element.

struct RemoveDuplicates

A publisher that publishes only elements that don’t match the previous element.

struct TryRemoveDuplicates

A publisher that publishes only elements that don’t match the previous element, as evaluated by a provided error-throwing closure.

struct ReplaceEmpty

A publisher that replaces an empty stream with a provided element.

struct ReplaceError

A publisher that replaces any errors in the stream with a provided element.

