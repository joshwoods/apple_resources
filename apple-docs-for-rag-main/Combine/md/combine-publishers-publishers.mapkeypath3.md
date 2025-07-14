

- Combine
- Publishers
-  Publishers.MapKeyPath3 

Structure

# Publishers.MapKeyPath3

A publisher that publishes the values of three key paths as a tuple.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct MapKeyPath3 where Upstream : Publisher
```

## Topics

### Declaring Publisher Topography

typealias Output

The kind of values published by this publisher.

typealias Failure

The kind of errors this publisher might publish.

### Inspecting Publisher Properties

let upstream: Upstream

The publisher from which this publisher receives elements.

let keyPath0: KeyPath&lt;Upstream.Output, Output0>

The key path of a property to publish.

let keyPath1: KeyPath&lt;Upstream.Output, Output1>

The key path of a second property to publish.

let keyPath2: KeyPath&lt;Upstream.Output, Output2>

The key path of a third property to publish.

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

struct MapKeyPath

A publisher that publishes the value of a key path.

struct MapKeyPath2

A publisher that publishes the values of two key paths as a tuple.

