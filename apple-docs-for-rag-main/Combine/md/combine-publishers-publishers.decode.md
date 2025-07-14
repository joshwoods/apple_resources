

- Combine
- Publishers
-  Publishers.Decode 

Structure

# Publishers.Decode

A publisher that decodes elements received from an upstream publisher, using a given decoder.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct Decode where Upstream : Publisher, Output : Decodable, Coder : TopLevelDecoder, Upstream.Output == Coder.Input
```

## Topics

### Creating a Decode Publisher

init(upstream: Upstream, decoder: Coder)

Creates a publisher that decodes elements received from an upstream publisher, using a given decoder.

### Declaring Publisher Topography

struct Output

A publisher that publishes elements specified by a range in the sequence of published elements.

typealias Failure

The kind of errors this publisher might publish.

### Inspecting Publisher Properties

let upstream: Upstream

### Applying Operators

Publisher Operators

Methods that create downstream publishers or subscribers to act on the elements they receive.

### Default Implementations

Publisher Implementations

## Relationships

### Conforms To

- Publisher

## See Also

### Encoding and Decoding

struct Encode

A publisher that encodes elements received from an upstream publisher, using a given encoder.

