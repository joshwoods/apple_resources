

- Combine
- Publishers
-  Publishers.ReplaceEmpty 

Structure

# Publishers.ReplaceEmpty

A publisher that replaces an empty stream with a provided element.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct ReplaceEmpty where Upstream : Publisher
```

## Topics

### Creating a Replace Empty Publisher

init(upstream: Upstream, output: Publishers.ReplaceEmpty&lt;Upstream>.Output)

Creates a publisher that replaces an empty stream with a provided element.

### Declaring Publisher Topography

typealias Output

The kind of values published by this publisher.

typealias Output

The kind of values published by this publisher.

typealias Failure

The kind of errors this publisher might publish.

### Inspecting Publisher Properties

let upstream: Upstream

The publisher from which this publisher receives elements.

let output: Publishers.ReplaceEmpty&lt;Upstream>.Output

The element to deliver when the upstream publisher finishes without delivering any elements.

let output: Publishers.ReplaceEmpty&lt;Upstream>.Output

The element to deliver when the upstream publisher finishes without delivering any elements.

### Comparing Publishers

static func == (Publishers.ReplaceEmpty&lt;Upstream>, Publishers.ReplaceEmpty&lt;Upstream>) -> Bool

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

### Filtering Elements

struct Filter

A publisher that republishes all elements that match a provided closure.

struct TryFilter

A publisher that republishes all elements that match a provided error-throwing closure.

struct CompactMap

A publisher that republishes all non-nil results of calling a closure with each received element.

struct TryCompactMap

A publisher that republishes all non-nil results of calling an error-throwing closure with each received element.

struct RemoveDuplicates

A publisher that publishes only elements that don’t match the previous element.

struct TryRemoveDuplicates

A publisher that publishes only elements that don’t match the previous element, as evaluated by a provided error-throwing closure.

struct ReplaceError

A publisher that replaces any errors in the stream with a provided element.

