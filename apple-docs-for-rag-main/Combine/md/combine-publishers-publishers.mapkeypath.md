

- Combine
- Publishers
-  Publishers.MapKeyPath 

Structure

# Publishers.MapKeyPath

A publisher that publishes the value of a key path.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct MapKeyPath where Upstream : Publisher
```

## Topics

### Declaring Publisher Topography

struct Output

A publisher that publishes elements specified by a range in the sequence of published elements.

typealias Failure

The kind of errors this publisher might publish.

### Inspecting Publisher Properties

let upstream: Upstream

The publisher from which this publisher receives elements.

let keyPath: KeyPath&lt;Upstream.Output, Output>

The key path of a property to publish.

### Applying Operators

Publisher Operators

Methods that create downstream publishers or subscribers to act on the elements they receive.

### Default Implementations

Publisher Implementations

## Relationships

### Conforms To

- Publisher

## See Also

### Identifying Properties with Key Paths

struct MapKeyPath2

A publisher that publishes the values of two key paths as a tuple.

struct MapKeyPath3

A publisher that publishes the values of three key paths as a tuple.

