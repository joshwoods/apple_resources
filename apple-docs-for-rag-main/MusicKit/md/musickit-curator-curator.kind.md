

- MusicKit
- Curator
-  Curator.Kind 

Enumeration

# Curator.Kind

The available kinds of curators.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 12.3+tvOS 15.4+visionOS 1.0+watchOS 9.0+

``` source
enum Kind
```

## Topics

### Operators

static func == (Curator.Kind, Curator.Kind) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case editorial

Indicates that the curator is an Apple Music curator.

case external

Indicates that the curator is an external, third-party curator.

### Initializers

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func encode(to: any Encoder) throws

Encodes this value into the given encoder.

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

