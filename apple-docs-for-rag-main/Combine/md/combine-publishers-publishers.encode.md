

- Combine
- Publishers
-  Publishers.Encode 

Structure

# Publishers.Encode

A publisher that encodes elements received from an upstream publisher, using a given encoder.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct Encode where Upstream : Publisher, Coder : TopLevelEncoder, Upstream.Output : Encodable
```

## Topics

### Creating a Encode Publisher

init(upstream: Upstream, encoder: Coder)

Creates a publisher that decodes elements received from an upstream publisher, using a given decoder.

### Declaring Publisher Topography

typealias Output

The kind of values published by this publisher.

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

struct Decode

A publisher that decodes elements received from an upstream publisher, using a given decoder.

